# Implementation Tasks

## Elevation

In the **Motion and elevation** section of [Depicting Elevation](https://material.io/design/environment/elevation.html#depicting-elevation), there are strategies for transitioning focus using elevation. These patterns would be very useful for working with elements. Their implementation would drastically improve the fluidity of our apps without impacting performance (as this motion is handled natively by the browser and incurs no penalties as a result of network latency).

## Layout

Within the primary layout of our apps, use the [Responsive layout grid](https://material.io/design/layout/responsive-layout-grid.html) concept, in conjunction with CSS Grid or CSS Flex, to manage the responsiveness of our app and the containment of elements within layouts.

> For instance, rather than explicitly constraining components with a width, have them fill across columns within the grid layout.

> See the following resources:
> * [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
> * [A Complete Guide to Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
> * [Algorithmic Layouts](https://css-tricks.com/algorithmic-layouts/)
> * [CSS Grid Starter Layouts](https://css-tricks.com/snippets/css/css-grid-starter-layouts/)
> * [Flexbox and Grids, your layout's best friends](https://css-tricks.com/flexbox-grids-layouts-best-friends/)
> * [Native CSS Masonry Layout in CSS Grid](https://css-tricks.com/native-css-masonry-layout-in-css-grid/)
> * [Approaches for a CSS Masonry Layout](https://css-tricks.com/piecing-together-approaches-for-a-css-masonry-layout/)
> * [Angular: Grid List](https://material.angular.io/components/grid-list/examples)

Integrate [Breakpoints](https://material.io/design/layout/responsive-layout-grid.html#breakpoints) into the theme styling to determine layout and appearance.

Establish core [UI Region](https://material.io/design/layout/responsive-layout-grid.html#ui-regions) based layouts for our modules + strategy for implementing the module menu within each app. Consider the guidelines outlined in the [Responsive Patterns](https://material.io/design/layout/component-behavior.html#responsive-patterns) section.

Consider how [Applying Density](https://material.io/design/layout/applying-density.html) to components and layouts can optimize the UX of our apps.

## Navigation

In addition to the above-mentioned **UI Region** and **Responsive Patterns** guidelines, consider how [Navigation](https://material.io/design/navigation/understanding-navigation.html) can be implemented in difference navigational scenarios across different layouts.

> See the following resources:
> * [Angular: Routing & Navigation](https://angular.io/guide/router)
> * [Angular Material: Bottom Sheet](https://material.angular.io/components/bottom-sheet/overview)
> * [Angular Material: Sidenav](https://material.angular.io/components/sidenav/overview)
> * [Angular Material: Tabs](https://material.angular.io/components/tabs/overview)

Use of motion to enable [Navigation Transitions](https://material.io/design/navigation/navigation-transitions.html).

> See the following resources:
> * [Using CSS Transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)
> * [`transition` reference](https://css-tricks.com/almanac/properties/t/transition/)
> * [Angular Animations](https://angular.io/guide/animations)

Color

Refine the extended color management features of our theming. Particularly, create a mixin that generates styles based on a provided collection of color palettes. The styles should account for:

* Foreground color
* Background color
* Border color
* Glow color

We should be able to create UI layouts that make more comprehensive use of colors:

![green-layout](https://lh3.googleusercontent.com/AUc8ae14K44qkCTWKOCz6dvgIEeih8h2t3v2Y8c6RVKxwyHuJjbY3FiY00De8vyyVyheqY42nk02Nw6ljfqcxCdm0_tQYb3NCkOvwQ=w1064-v0)

![violet-layout](https://lh3.googleusercontent.com/qNrXgxomfHYbh8K-TWq0iAcyheIGWdhe5BjIEdBmHibR6ug3ZsOrsANiIqXwOF_IxHQN52QUBKpprb4GYQPwg9Ch9YPl4zd7FhUdiA=w1064-v0)

![blue-layout](https://lh3.googleusercontent.com/4xogmeEZv0K7ZyAVZy87v4nWAPpaIPLDVgGcIan5BFGY83lyJP3ybSTxIC8rSWMnCQV4gEo-9U79Yt4M8f7HgnixBvNqXb1yeXEJ=w1064-v0)

> See the following resources:
> * [Sass: String Interpolation](https://sass-lang.com/documentation/interpolation)
> * [Sass: Maps](https://sass-lang.com/documentation/values/maps)
> * [Sass: @mixin](https://sass-lang.com/documentation/at-rules/mixin)
> * [Angular Components: _palette.scss](https://github.com/angular/components/blob/master/src/material/core/theming/_palette.scss)
> * [Angular Components: _theming.scss](https://github.com/angular/components/blob/master/src/material/core/theming/_theming.scss)

Establish guidelines for [glow](https://github.com/JaimeStill/design-study/tree/master/examples/glowing-elevation) based on the notion that Material recommends [not using light glows in place of dark shadows to express elevation](https://material.io/design/color/dark-theme.html#properties) (see the Elevation section within this link).

Revisit our platform's theme colors, and verify based on the [Material guidelines](https://material.io/design/color/dark-theme.html#ui-application).

## Iconography

Potentially look at (making Phil) design icons for the app modules, based on the [Product icons guidelines](https://material.io/design/iconography/product-icons.html#design-principles).