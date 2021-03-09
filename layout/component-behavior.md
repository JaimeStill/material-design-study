# Component Behavior

The following guidance describes how components behave, both in the grid and between breakpoints.

## Positioning Terminology

UI elements behave in different ways at each breakpoint range.

### Descriptors

The position of UI elements, components, and surfaces in the grid can be described using the following terms:

Descriptor | Definition
-----------|-----------
Above, below | The y position of an element
In front of, behind | The z position of an element
Left, right, centered | The x position of an element
Top, bottom | The y position of an element relative to a container or screen edge
Vertically centered | The x and y position of an element are centered relative to a container or screen edges
Sticky | An element that scrolls with the UI and locks at a certain point in the scroll position
Floating | A fixed element positioned in front of scrolling content

## Component Width

Compnent width can remain the same across screen sizes, or it can change depending on the layout. Component width can be either:

* Fixed
* Fluid

Because fixed width elements retain their width during layout changes, their placement can change to accomodate new layouts. Their placement can be either:

* Pushed
* Overlaid

### Fixed

When an element has a fixed width, its width stays the same even across screen size changes.

### Fluid

When an element has a fluid width, its width expands and contracts as the screen size changes.

> Don't use a container on fluid components if it's too narrow to display elements and padding at smaller widths.

> Use caution when spanning a fluid component across several columns in a wide screen. Certain components, like buttons, might be overly emphasized on larger screen widths.

### Push

When layout and screen size change, a component can be pushed from its original position. Component width remains the same, but its position changes horizontally, moving left or right. When this occurs, it may be partially occluded by a screen's edge if pushed off-screen.

### Overlaid

When a UI changes, a component can be overlaid by other elements that occlude it. When a component is overlaid, its width and position remain the same.

## Responsive Patterns

Components can adapt their dimensions based on screen size and device type, using the following patterns. These dimension adaptations can include:

* Using different components that fit the space better
* Altering the visibility of components to accomodate smaller spaces
* Changing to input methods

As screen space increases, the following responsive patterns may be applied.

### Reveal

Parts of the UI hidden by smaller screens can be revealed when additional space becomes available at a designated breakpoint.

Elements, such as side navigation, can become visible when screen size increases:

![side-nav-reveal](https://lh3.googleusercontent.com/LbLFh1meWGfpWysnb06PxAWZ7AKAQvVmjft3sGjwxmLh6dFbH6KlGDHlP3aXah18VB_cZdSlQOp_BO26hq47cf4i_6XVQnjewubDYg=w1064-v0)

A simple UI may reveal more robust or complex options:

![complex-ui-reveal](https://lh3.googleusercontent.com/FUpEK178Gn5lbtXqEA3XCIgYnJ48XBaH566CSJFSjuuM_ArLKgcDA-La1ylucc3NcIBMGYxkxOSxbe7Yv5Rpe-EUTvr_EcuoseWIdA=w1064-v0)

Content that only appears after tapping on a small screen can be revealed by default when more space is available:

![extended-content-reveal](https://lh3.googleusercontent.com/i0KKJDrE0FriDD-FbCnwSksHqJex3797QS34pYsPA8nmQb0qu6ugWUnmRSRCgTMkrzX8gib-xP-sFU8EzfTr-Kj-jk8TFVaNAPdJ2g=w1064-v0)

### Transform

A component can trasnform from one format to another at a designated breakpoint.

Side navigation can transform into tabs on a larger screen:

![nav-transform](https://lh3.googleusercontent.com/fgljRRWmOxyCOh7x2li4tN7ZV9A3t6FC28aYhk3xWe-aLgMobI6Z0Q0ekJIaZI-tYsUZrPaNtLt5Or9iExBx-E8htOoqpDizIeY2=w1064-v0)

A list can transform into an image list on a larger screen:

![list-transform](https://lh3.googleusercontent.com/qQClrwn6U_wEzJG5lKInIhrpo1abd_9ycIbC5B0Msqm4k_sp2N3lnRX7mCxHvy0vb_qMwu0P22R8UqSB3-yG8_6lpfFiNvpwP_mQOjM=w1064-v0)

Menu items can transform into icons on a toolbar on a larger screen:

![menu-transform](https://lh3.googleusercontent.com/yIz2fohPNJxU-av1vEKq5skvS4jjCCS0lgbn2ITII7f7VFDKG5pGmAaiQ7taMt505JX4rXxkkZYIO85GvG6VCIN93tS7lOXAi9IyrQ=w1064-v0)

### Divide

UIs with multiple layers can display all of those layers at once when more screen space is available. UI elements are divided across this newly available space.

Side navigation, list content, and detailed content divide to fill a single view on a larger screen:

![nav-and-list-divide](https://lh3.googleusercontent.com/si5L6YyF3kxu4r7j-dRtollIeaHj5DBN6UyTwvgTksRQ3Si_Cz5BXAHl-MUGG4mJmPNeU9iCVpPYTf-ZXokTj2y8crOJ9GchrkMBeag=w1064-v0)

Tabbed sibling content is divided within the same view on a larger screen.

![tab-divide](https://lh3.googleusercontent.com/arj45MoELjYMAIi7XMBD69u06hj_osmk_Excobn86zGoOXSOsrtzL7z3SXUvIT1gsVJaqrN_J5xpirMR9WO5HnS61se3aDO98HjKhQ=w1064-v0)

### Reflow

A UI may change its layout to reflow across newly available space.

Elements from a single-column format can reflow to fill the content area in various combinations on a larger screen:

![column-reflow](https://lh3.googleusercontent.com/lgHcP_d4dDLitEW-MCJHj3J8Pt8Tj99gA_F8FvpcgU_FmuMYI9FYNJhR2n9jf15f94joUtDvNSoU6Mr54r9g_PENAdu7_EjzwmCf=w1064-v0)

Horizontal tabs can reflow into a vertical list on a larger screen:

![vertical-list-reflow](https://lh3.googleusercontent.com/FkVg5C4HSUdi5Gjqr2-jUCjN-O73iU-Nn-jF38bQmPw5LZuz4vgg6_1V63upu-2TCzucTv_Pcwu62iAE0Hzeo_wWIYPH5tll7ThVpXY=w1064-v0)

Elements can reflow within a component based on a new screen ratio or device orientation:

![component-reflow](https://lh3.googleusercontent.com/PQ8CtuEY2VQi0QeKs-8bXAeJnuU_FgvJhYeliXvk5qOuWBV28FJYIxWag6FP2jP8AQ6OkaHvtF794oHiBpYyowaqXPo8VdllWMKYwm4=w1064-v0)

### Expand

The UI can expand across more space.

Cards can expand to fill a new and larger space:

![card-expand](https://lh3.googleusercontent.com/4m_eMtkSTTpgNCwC0YrZK0rlBI_fZgIssl4V48uuVsdeW9TYJ8M3fUzaU8uqnAT-7p2rh4kgGQcDMRdil9naQabvcRDpb5B9mmp6=w1064-v0)

Dialogs can expand proportionally with content or in specific increments:

![dialog-expand](https://lh3.googleusercontent.com/o6gGy_ZOpsuUfTznw8ooHvzt91POO70dCZa8H-6jq10yQfbp2qPCCqhN-IzN-Uepp890pWaXrCf8B5RdvyY2d5NJBuFIy_HtAPSzHQQ=w1064-v0)

### Position

The position of UI components can change to more appropriate locations.

A bottom sheet on a small screen can reposition itself as a menu on a larger screen:

![menu-position](https://lh3.googleusercontent.com/W26FX-XRwmshjmltbV46zgPsOGfJlGWJdt_T_E8oKiddywKIyvCHA0clRYvGf8vzo-9BKpaXZBFU0dWmOwpFoD3cexgajxnLmpf7iw=w1064-v0)

A floating action button (FAB) can move to a more visible location relative to other UI elements on a larger screen:

![fab-position](https://lh3.googleusercontent.com/Kdj_z_th6eCNiKaWfVtPlRNjD5J3Ap04mj_LYHsr-zOt41oRx7u41DwRy24bygYzZExfYCje-Upe7jn5VjA6ryZsG_hHKe--HXQX3a4=w1064-v0)