# Measurements

Material Design layouts are visually balanced. Most measurements align to an 8px grid applied, which aligns both spacing and the overall alyout.

Smaller components, such as icons and type, can align to a 4px grid.

![material-measurements](https://lh3.googleusercontent.com/lNSGNuRb8_y3w6y2gFEBprF4oyGsC0nM7wAVW3NirOoxWwpvz-MKFnO0C2hZ6d3gTbi7BO9DYWUtznmd_7qtnzjKGiUDMKvfFtpRGA=w1064-v0)

## Pixel Density

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

## Density Independence

Density-independent pixels, written as dp (pronounced "dips"), are flexible units that scale to have uniform dimensions on any screen. They provide a flexible way to accommodate a design across platforms. Material UIs use density-independent pixels to display elements consistently on screens with different densities.

![density-independence](https://lh3.googleusercontent.com/_SO3kwOpx8F0MzIkb0z0q7paNqPMK3v_wtL7Es1oBKdN__aejeV5gw261UX1XST6refOBlbOaNwXvPaO-PKGRUiZX_moClbcYA_Q=w1064-v0)

1. Low-density screen displayed with density independence
2. High-density screen displayed with density independence

## Pixel Density on the Web

**Logical Resolution** - Use the device's logical resolution, which scales to the device's screen resolution.

**Units for the web** - When designing for the web, replace dp with px (for pixel).