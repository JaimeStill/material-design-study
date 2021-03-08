# Responsive Layout Grid

The Material Design responsive layout grid is an overarching guide to the placement of components and elements. The responsive layout grid adapts to screen sizes and orientation, ensuring consistency across layouts. It is made up of three elements: columns, gutters, and margins.

![layout-grid](https://lh3.googleusercontent.com/r6fKrpfXlzXvGokFAgYHp_FE3JRXT4GLoSMPqzQqB4R-wMHYqc94xyHnF0IE4Ndtfmc6BvDBockiOSVnbdTohlj6ftAlV2mLjevy=w1064-v0)

1. Columns
2. Gutters
3. Margins

## Columns

Content is placed in the areas of the screen that contain columns. Column width is defined using percentages, rather than fixed values, to allow content to flexibly adapt to any screen size. The number of columns displayed in the grid is determined by the breakpoint range (a range of predetermined screen sizes) at which a screeen is viewed, whether it's a breakpoint for mobile, tablet, or another size.

On mobile, a breakpoint of 360dp, this layout grid uses 4 columns:  

![mobile-columns](https://lh3.googleusercontent.com/D6pd4WU4-5xxx08GxsMY-v-g8Di9n1vHCYdmnKw8R-4xIbPm-HSjnXXOI2hgyEn_S8uRzR9c2KNowRdQRJuyAAcoQ5xmoPhIKKh-=w1064-v0)

On tablet, at a breakpoint of 600 dp, this layout grid uses 8 columns:  

![tablet-columns](https://lh3.googleusercontent.com/82njrJBKzXerg8zX_V8GPhLEH1QkHyzCXj3f7-330MTurhxvvrEsHofEgsMuLVW2_Ts5ctJ-OSM2zSfdKN0SnL84R64T9upojLxK=w1064-v0)

## Gutters

Gutters are the spaces between columns. They help separate content. Gutter widths are fixed values at each breakpoint range. To better adapt to the screen, gutter width can change at different breakpoints. Wider gutters are more appropriate for larger screens, as they create more whitespace between columns.

On mobile, at a breakpoint of 360 dp, this layout grid uses 16dp gutters:  

![mobile-gutters](https://lh3.googleusercontent.com/lDP0K31FpCQxQsctqnCE9kfoEZEHA-y0-agvkZxgVuwp0j6hXoV1VZp8CmnhK_RaFYoo1wvW93Fs-q4yWg-8eYsSKb2gLLfFeFSKGw=w1064-v0)

On tablet, at a breakpoint of 600 dp, this layout grid uses 24dp gutters:  

![tablet-gutters](https://lh3.googleusercontent.com/CZEGEUX6NSCLGHrlN0W3KGJ3SvG4HTgE_Z1OXgrLaxYE3Zku2MuO7mfby1m-6wrzIKD1kp25H1iXhjO4te2AbHRJf2bripFdnrkx=w1064-v0)

## Margins

Margins are the space between contont and the left and right edges of the screen. Margin widths are defined as fixed values at each breakpoint range. To better adapt tot he screen, the margin width can change at different breakpoints. Wider margins are more appropriate for larger screens, as they create more whitespace around the perimeter of content.

On mobile, at a breakpoint of 360 dp, this layout grid uses 16dp margins:  

![mobile-margins](https://lh3.googleusercontent.com/zs_TXfpOmkPDHRzVllD9ddlI4gVfLRGTV7qS4sBW0sE0Wer3RUgT6dClsKcVlRyNBY2cCDfd65OzPI7FqjsUzFvtxO8NmivYjFOOrg=w1064-v0)

On tablet, at a breakpoint of 600 dp, this layout grid uses 24dp margins:  

![tablet-margins](https://lh3.googleusercontent.com/7EV1c2B2UqqkjDmRK4eNN6mTd9Yy3-ajxmVbxtS_gXzMRxuFPK2PKMWPwh6Vh1nb2ApsIYFg042BbKnvAsCM0fPDxNDnLJWvqBWl-Ic=w1064-v0)

## Breakpoints

A breakpoint is the range of predetermined screen sizes that have specific layout requirements. At a given breakpoint range, the layout adjusts to suit the screen size and orientation.

Material Design provides responsive layouts based on the following column structures. Layouts using 4-column, 8-column, and 12-column grids are available for use across different screens, devices, and orientations.

Each breakpoint range determines the number of columns, and recommended margins and gutters, for each display size.

Breakpoint Range (dp) | Portrait | Landscape | Window | Columns | Margins / Gutters*
----------------------|----------|-----------|--------|---------|------------------
0 - 359 | small handset | | xsmall | 4 | 16
360 - 399 | medium handset | | xsmall | 4 | 16
400 - 479 | large handset | | xsmall | 4 | 16
480 - 599 | large handset | small handset | xsmall | 4 | 16
600 - 719 | small tablet | medium handset | small | 8 | 16
720 - 839 | large tablet | large handset | small | 8 | 24
840 - 959 | large tablet | large handset | small | 12 | 24
960 - 1023 | | small tablet | small | 12 | 24
1024 - 1279 | | large tablet | medium | 12 | 24
1280 - 1439 | | large tablet | medium | 12 | 24
1440 - 1599 | | | large | 12 | 24
1600 - 1919 | | | large | 12 | 24
1920+ | | | xlarge | 12 | 24

* *Margins and gutters are flexible and don't need to be of equal size*

## Grid Behavior

### Fluid Grids

Fluid grids use columns that scale and resize content. A fluid grid's layout can use breakpoints to determine if the layout needs to change dramatically.

### Fixed Grids

Fixed grids use columns of a fixed size, with fluid margins to keep content unchanging within each breakpoint range. A fixed grid's layout can only change at an assigned breakpoint.

## UI Regions

A layout is made up of several UI regions, such as side navigation, content areas, and app bars. These regions can display actions, content, or navigation destinations. UI regions should be consistent across devices, whil adapting to different breakpoints of different screen sizes.

To increase familiarity across devices, UI elements designed for desktop should be organized in a way that's consistent wtih the mobile UI.

### Permanent UI Regions

Permanent UI regions are regions that can be displayed outside of the responsive grid, like a navigation drawer. These regions cannot be collapsed.

### Persistent UI Regions

Persistent UI regions are regions that can be displayed upon command at any time, or they can remain visible. They can be toggled on or off, to appear or disappear. When they appear, they condense both content and the grid.

When a persistent UI region is visible, its visibility isn't affected by interaction with other elements on screen.

### Temporary UI Regions

Temporary UI regions appear temporarily, and when they do, they do not affect the responsive grid. When visible, they can be hidden by tapping an item in their region, or any space outside of their region.

When a UI region is visible, other screen elements aren't interactive.