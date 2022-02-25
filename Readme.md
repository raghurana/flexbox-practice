## Axis

- main axis (if flex-direction is row, this would be horizontal line)
- cross axis (vertical for flex-direction row)

## Flex Directions

- **row** - content will flow horizontally
- **column** - conent will flow veritically
- **rowreverse** - content will be rendered in the reverse order of how it was added, horizontally

## Content alignment

- **justify-content** will work on the main axis
  - **center** - would align content to middle for flex-direction row.
  - **flex-start** - align content to very beginning of the main axis
  - **flex-end** - align content to end of the main axis
  - **space-between** - make equal space between all the boxes
  - **space-around** - equal space between inner boxes, half on the first and last boxes

> Note - In space-evenly, the empty space in between the flex items is always equal. However, in space-around, only the inner items will have equal spacing in between each other. The first and last item will only be allocated half the spacing.

- **align-items** will work on the cross axis on each flex item/box

  - **strecth** - default value. If one of the boxes is bigger tha other, them all content is strected to fill the parent.
  - **center** - will vertically align boxes to center of parent if flex direction is row
  - **flex-start** - align content to very beginning of the cross axis
  - **flex-end** - align content to end of the cross axis
  - **baseline** - align items cross axis based on the text inside the boxes.

- **align-self** will work on the cross axis

  - similar values to align items, but can be applied to individual box

- **align-content** (_multi-row container_) applies to the entire content of the flex container as opposed to individual items. align-content doesn't interfere with items in a row but with rows itself. Hence, align-content will try to align rows with respect to each other and flex container. Doesnt have effect on single row containers. Default the value is stretch, but all values of align-items can work here too.

## Content ordering

By default all boxes have an order value of 0, if flex-direction is row and you wnat to move b2 to first position, set its order to -1 and similarly to move b4 to end set its order to 1

## Content expansion/contraction

- **flex-grow** - setting value to 1 (default) will cause a box to take as much space as available along the main axis. Setting it to 0 will prevent any growth.
- **flex-shrink** - by default the value is 1, that allows a box to be responsive. Setting this to 0 will prevent box from shrinking.
- **flex-basis** - initial width of a box along the main axis, can be % or px or auto. If flex-grow and flex-shrink properties are both set to 1 on all flex-items/boxes, then flex items can grow and shrink from the initial flex-basis.
  **auto** means look at my height and width propeties
  **content** means look at my content size itself

  > Shorthand for all three above is `flex: <grow> <shrink> <basis>`

By Default if there are more flex items than the width of the flex container (main) then items will overflow with a horizontal scrollbar (flex-direction row)> this can be fixed with flex-wrap

- **flex-wrap** - by default **nowrap**, but **wrap** will wrap contents along the main axis. Also has a **wrap-reverse**
