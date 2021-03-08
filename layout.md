# Layout  

* [Principles of Layout](#principles-of-layout)
* [Material Measurements](#material-measurements)
* [Pixel Density](#pixel-density)
    * [Calculating Pixel Density](#calculating-pixel-density)
    * [Density Independence](#density-independence)
    * [Pixel Density on the Web](#pixel-density-on-the-web)
* [Responsive Layout Grid](#responsive-layout-grid)
    * [Columns](#columns)
    * [Gutters](#gutters)
    * [Margins](#margins)


Material Design layouts encourage consistency across platforms, environments, and screen sizes by using uniform elements and spacing.

## Principles of Layout
[Back to Top](#layout)

**Predictable** - Use intuitive and predictable layouts with consistent UI regions and spatial organization.  
**Consistent** - Layouts should be consistent in the use of grids, keylines, and padding.  
**Responsive** - Layouts are adaptive and they react to input from a user, a device, and screen elements.

## Material Measurements
[Back to Top](#layout)

Material Design layouts are visually balanced. Most measurements align to an 8px grid applied, which aligns both spacing and the overall alyout.

Smaller components, such as icons and type, can align to a 4px grid.

![material-measurements](https://lh3.googleusercontent.com/lNSGNuRb8_y3w6y2gFEBprF4oyGsC0nM7wAVW3NirOoxWwpvz-MKFnO0C2hZ6d3gTbi7BO9DYWUtznmd_7qtnzjKGiUDMKvfFtpRGA=w1064-v0)

## Pixel Density
[Back to Top](#layout)

The number of pixels that fit into an inch is referred to as pixel density. High-density screens have more pixels per inch than low-density ones. As a result, UI elements of the same pixel dimensions appear larger on low-density screens, and smaller on high-density screens.

### Calculating Pixel Density

To calculate screen density, you can use the following equation:

```
Screen density = Screen width (or height) in pixels / Screen width (or height) in inches
```

**High-density Display**  

![high-density-display](https://lh3.googleusercontent.com/NXbwdWYdlNMs5HA7tv-CCTtIiW2-96XHMpydZ4_M7SxFSMx2KYug3z-nBBQXGGhC0JVxhrL6CX0yP2fdzoXC4t783uzqFC_xQAM8JIM=w1064-v0)

**Low-density Display**  

![low-density-display](https://lh3.googleusercontent.com/RNAucz3HiKbTVhEz1fUBJzTorwRhe0-f4Y37WeLiojhoI2dhwDWo-afpOt6drgIjA99AgEtg1_NEgvc-hfnVUocGkwsKKYCwSV0h=w1064-v0)

### Density Independence
[Back to Top](#layout)

Density-independent pixels, written as dp (pronounced "dips"), are flexible units that scale to have uniform dimensions on any screen. They provide a flexible way to accommodate a design across platforms. Material UIs use density-independent pixels to display elements consistently on screens with different densities.

![density-independence](https://lh3.googleusercontent.com/_SO3kwOpx8F0MzIkb0z0q7paNqPMK3v_wtL7Es1oBKdN__aejeV5gw261UX1XST6refOBlbOaNwXvPaO-PKGRUiZX_moClbcYA_Q=w1064-v0)

1. Low-density screen displayed with density independence
2. High-density screen displayed with density independence

### Pixel Density on the Web
[Back to Top](#layout)

**Logical Resolution** - Use the device's logical resolution, which scales to the device's screen resolution.

**Units for the web** - When designing for the web, replace dp with px (for pixel).

## Responsive Layout Grid
[Back to Top](#layout)

The Material Design responsive layout grid is an overarching guide to the placement of components and elements. The responsive layout grid adapts to screen sizes and orientation, ensuring consistency across layouts. It is made up of three elements: columns, gutters, and margins.

![layout-grid](https://lh3.googleusercontent.com/r6fKrpfXlzXvGokFAgYHp_FE3JRXT4GLoSMPqzQqB4R-wMHYqc94xyHnF0IE4Ndtfmc6BvDBockiOSVnbdTohlj6ftAlV2mLjevy=w1064-v0)

1. Columns
2. Gutters
3. Margins

### Columns
[Back to Top](#layout)

Content is placed in the areas of the screen that contain columns. Column width is defined using percentages, rather than fixed values, to allow content to flexibly adapt to any screen size. The number of columns displayed in the grid is determined by the breakpoint range (a range of predetermined screen sizes) at which a screeen is viewed, whether it's a breakpoint for mobile, tablet, or another size.

On mobile, a breakpoint of 360dp, this layout grid uses 4 columns:  

![mobile-columns](https://lh3.googleusercontent.com/D6pd4WU4-5xxx08GxsMY-v-g8Di9n1vHCYdmnKw8R-4xIbPm-HSjnXXOI2hgyEn_S8uRzR9c2KNowRdQRJuyAAcoQ5xmoPhIKKh-=w1064-v0)

On tablet, at a breakpoint of 600 dp, this layout grid uses 8 columns:  

![tablet-columns](https://lh3.googleusercontent.com/82njrJBKzXerg8zX_V8GPhLEH1QkHyzCXj3f7-330MTurhxvvrEsHofEgsMuLVW2_Ts5ctJ-OSM2zSfdKN0SnL84R64T9upojLxK=w1064-v0)

### Gutters
[Back to Top](#layout)

Gutters are the spaces between columns. They help separate content. Gutter widths are fixed values at each breakpoint range. To better adapt to the screen, gutter width can change at different breakpoints. Wider gutters are more appropriate for larger screens, as they create more whitespace between columns.

On mobile, at a breakpoint of 360 dp, this layout grid uses 16dp gutters:  

![mobile-gutters](https://lh3.googleusercontent.com/lDP0K31FpCQxQsctqnCE9kfoEZEHA-y0-agvkZxgVuwp0j6hXoV1VZp8CmnhK_RaFYoo1wvW93Fs-q4yWg-8eYsSKb2gLLfFeFSKGw=w1064-v0)

On tablet, at a breakpoint of 600 dp, this layout grid uses 24dp gutters:  

![tablet-gutters](https://lh3.googleusercontent.com/CZEGEUX6NSCLGHrlN0W3KGJ3SvG4HTgE_Z1OXgrLaxYE3Zku2MuO7mfby1m-6wrzIKD1kp25H1iXhjO4te2AbHRJf2bripFdnrkx=w1064-v0)

### Margins
[Back to Top](#layout)

