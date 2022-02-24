## Axis

- main axis (if flex-direction is row, this would be horizontal line)
- cross axis (vertical for flex-direction row)

## Flex Directions

- **row** - content will flow horizontally
- **column** - conent will flow veritically
- **rowreverse** - content will be rendered in teh reverse order of how it was added

## Content alignment

- **justify-content** will work on the main axis
  - **center** - would align content to middle for flex-direction row.
  - **flex-start** - align content to very beginning of the main axis
  - **flex-end** - align content to end of the main axis
  - **space-between** - make equal space between all the boxes
  - **space-around** - equal space between inner boxes, half on the first and last boxes

> Note - In space-evenly, the empty space in between the flex items is always equal. However, in space-around, only the inner items will have equal spacing in between each other. The first and last item will only be allocated half the spacing.
