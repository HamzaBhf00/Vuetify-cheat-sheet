# Vuetify-cheat-sheet

<!-- Styles -->
1. Breakpoint:
   - Example: <v-btn class="xs-only">Visible on extra-small screens</v-btn>
   - Explanation: This button will only be visible on extra-small screens (xs breakpoint).

<!-- Display -->
2. .d-{value}:
   - Example: <v-dialog v-if="showDialog" class="d-none">Hidden Dialog</v-dialog>
   - Explanation: The dialog is hidden using the `d-none` class until `showDialog` is true.

3. .d-{breakpoint}-{value}:
   - Example: <v-img class="d-sm-inline d-xl-none">Responsive Image</v-img>
   - Explanation: This image is inline on small screens and hidden on extra-large screens.

<!-- Flex -->
4. Flex direction:
   - Example: <v-row class="flex-row">Horizontal Row</v-row>
   - Explanation: The row's items will flow horizontally.

5. Flex justify:
   - Example: <v-container class="justify-center">Centered Container</v-container>
   - Explanation: The container's content is centered horizontally.

6. Flex align:
   - Example: <v-col class="align-end">Bottom-aligned Column</v-col>
   - Explanation: The column is aligned to the bottom vertically.

7. Flex align self:
   - Example: <v-btn class="align-self-start">Top-aligned Button</v-btn>
   - Explanation: This button is aligned to the top within its container.

8. Flex wrap:
   - Example: <v-row class="flex-wrap">Wrapped Row</v-row>
   - Explanation: The row's items wrap to the next line as needed.

9. Flex order:
   - Example: <v-col class="order-2 order-md-1">Second on Mobile, First on Desktop</v-col>
   - Explanation: The column has a different order on mobile and desktop.

10. Flex align content:
    - Example: <v-row class="align-content-center">Centered Lines</v-row>
    - Explanation: Multiple lines within the row are centered vertically.

<!-- Float -->
11. .float-{value}:
    - Example: <v-btn class="float-left">Float Left</v-btn>
    - Explanation: The button floats to the left within its container.

<!-- Typography -->
12. Text alignment:
    - Example: <v-btn class="text-right">Right Aligned Button</v-btn>
    - Explanation: The button's text is right-aligned.

13. Text decoration:
    - Example: <v-span class="text-decoration-underline">Underlined Text</v-span>
    - Explanation: The text has an underline decoration.

14. Text wrapping and overflow:
    - Example: <v-paragraph class="text-truncate">This text will truncate if it overflows</v-paragraph>
    - Explanation: The text will truncate and display ellipsis if it overflows its container.

15. Text transform:
    - Example: <v-caption class="text-uppercase">Uppercase Caption</v-caption>
    - Explanation: The text is transformed to uppercase.

16. Text opacity:
    - Example: <v-span class="text--primary">Primary Text (87% opacity)</v-span>
    - Explanation: The text has a primary color with 87% opacity.

<!-- Font weights -->
17. Font weights:
    - Example: <v-span class="font-weight-bold">Bold Text</v-span>
    - Explanation: The text is styled with a bold font weight.
<!-- Spacing -->
18. Spacing (Margin and Padding):
    - Example: <v-card class="m-2 p-4">Card with Margin and Padding</v-card>
    - Explanation: The card has a margin of 8px and padding of 16px on all sides.

19. Spacing (Direction and Size):
    - Example: <v-row class="mt-3 pb-2 pl-5 s-4 e-6">Row with Custom Spacing</v-row>
    - Explanation: The row has top margin of 12px, bottom padding of 8px, left padding of 24px (in LTR mode), and right padding of 32px (in RTL mode).

20. Spacing (Size):
    - Example: <v-divider class="mb-0 n1">Negative Margin Divider</v-divider>
    - Explanation: The divider has a negative bottom margin of 4px.

<!-- Typography -->
21. Text alignment:
    - Example: <v-btn class="text-center">Center Aligned Button</v-btn>
    - Explanation: The button's text is center-aligned.

22. Text decoration:
    - Example: <v-span class="text-decoration-line-through">Strikethrough Text</v-span>
    - Explanation: The text has a strikethrough decoration.

23. Text wrapping and overflow:
    - Example: <v-paragraph class="text-wrap">This text will wrap within its container</v-paragraph>
    - Explanation: The text wraps when it reaches the container's edge.

24. Text transform:
    - Example: <v-caption class="text-capitalize">capitalized caption</v-caption>
    - Explanation: The text is transformed to capitalize the first letter of each word.

25. Text opacity:
    - Example: <v-span class="text--secondary">Secondary Text (60% opacity)</v-span>
    - Explanation: The text has a secondary color with 60% opacity.

26. Font weights light:
    - Example: <v-paragraph class="font-weight-light">Light Weight Text</v-paragraph>
    - Explanation: The text is styled with a light font weight.
<!-- Typography -->
27. Font weights medium:
    - Example: <v-paragraph class="font-weight-medium">Medium Weight Text</v-paragraph>
    - Explanation: The text is styled with a medium font weight.

28. Font weights black:
    - Example: <v-span class="font-weight-black">Black Weight Text</v-span>
    - Explanation: The text is styled with a black font weight.

29. Font weights thin:
    - Example: <v-span class="font-weight-thin">Thin Weight Text</v-span>
    - Explanation: The text is styled with a thin font weight.

30. Font weights regular:
    - Example: <v-span class="font-weight-regular">Regular Weight Text</v-span>
    - Explanation: The text is styled with a regular font weight.

31. Font weights bold:
    - Example: <v-span class="font-weight-bold">Bold Weight Text</v-span>
    - Explanation: The text is styled with a bold font weight.
