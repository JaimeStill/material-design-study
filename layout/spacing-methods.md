# Spacing Methods

Spacing methods use baseline grids, keylines, padding, and incremental spacing to adjust ratios, containers, and touch targets.

## Baseline Grid

**8dp grid**  

All components align to an 8dp square baseline grid for mobile, tablet, and desktop.

![baseline-grid](https://lh3.googleusercontent.com/uinGeklHxk33_lRawJUwCctxCz3QZXhpdYP27NaX8oFG_UmecEl56Ww9WK3qMmTc_dHAXcNFXyINLRHbJinylMuivSmjkTA6BNvyig=w1064-v0)

***

**4dp grid**

Icons, type adn some elements within components can align to a 4dp grid.

![icon-grid](https://lh3.googleusercontent.com/Cqdbcwkst0ekoN9nILUviSkOPFgz0l3-QNgboUrPZeYG4kG6SQ8-7K2juhT-GaOhP7OF7vKe87Y5oXl6p2OoE_EYu5pLzc6J5rMhag=w1064-v0)

***

**4dp baseline grid**

Type aligns to the 4dp baseline grid.

![typography-grid](https://lh3.googleusercontent.com/K_UG3A7jm8zmsW9BDuifTUTZDUeJK9YV3vcF8nELPdaozCGvAlJjev3Agvf43_84Nh9X7TR5ACGbFirQWLoWStPNivlA5u_RvTYdNA=w1064-v0)

Type can be placed outside of the 4dp grid when it's centered within a component, such as a button or list item. When placed outside of the grid but centered within a component, texc can still appear vertically center-aligned.

The text appears vertically aligned in the center of the list item, though the type is placed outside of the 4dp grid:

![vertically-centered-text](https://lh3.googleusercontent.com/Ryi55q2xjGwPEk9-VizBHTzmDtwfHnYRz3L5n9wfm8q7IgwqdWo7ilisFZpZcMYFCAJwef3XiHr8RC7rCgU07Tenyg_K8p36kFehkw=w1064-v0)

## Spacing

### Spacing Methods

Spacing methods are more granular than the responsive layout grid. Spacing methods are a set of rules around how to place elements within layouts and components.

#### Padding

![padding](https://lh3.googleusercontent.com/7oz4_mqkzr-lmSZciE3t7-ypIohWtD9k5cgVBNgt_SlCSRgSZV3NP6y8-HFLzOapEwJNJ5tcenFYtne2DeSdLrwa9TRWl6Wbxnv4=w1064-v0)

Padding is the space between elements within a component.

#### Dimensions

![dimensions](https://lh3.googleusercontent.com/fpL1dTOlSo2gc1ajP2msg1goP9LYCVEQ5Ikv5xaUkSnKAm_9tDy6AqXdjHZUHEuLjn4nnSBllpoBhRtasY26q8lgAtgFOPYmEtPAwg=w1064-v0)

Dimensions describe the width and height of component elements.

#### Alignment

![alignment](https://lh3.googleusercontent.com/PHRyk0W-Eb00cZ0AtrxXMvQczskDEIZzUDBHZHem3JU-ct6bGmt4rT5PWeP5JuNjl1KBDoZ4achUDCCDkoH7gQtCGb35X2jritte=w1064-v0)

Alignment is the placement of elements within a component.

### Padding

Padding refers to the space between UI elements. Padding is an alternative spacing method to keylines and is measured in increments of 8dp or 4dp.

Padding can be measured both vertically and horizontally and does not need to span the whole height of a layout.

A layout with 24dp padding between components:

![padding-layout](https://lh3.googleusercontent.com/uLOWkiGXp0rKOvpk1GY6p1ogxbCp31lmeDa23c_HIjsc4OBI_6cKNgXtOWBJJ6awV7QokMcXAKNuJLr1IOlc39DKv65MvV_s-zoNwNw=w1064-v0)

### Dimensions

Dimensions refer to the width and height of component elements. Some components, such as an app bar or list only outline the height of an element. The heights of these elements should align to the 8dp grid. Their widths are not specified because it's responsive to a viewport width.

![dimension-layout](https://lh3.googleusercontent.com/aI-9g5bMKLQVPquLTGARrO5UBuUeSbOUN8wA2spP7C86xGA-eIDhm_sMmwddVapYfV422RWJzg1ULUHdppKcX1hd-qg1axw0ahh7jw=w1064-v0)

1. Status bar height: 24dp
2. App bar height: 56dp
3. List item height: 88dp

### Alignment

Alignment is the placement of elements within a component.

![alignment-layout](https://lh3.googleusercontent.com/mQ64ispggPXYuhYJlWNMlpvtGXt4IfoqZ4Ns2BbfVKMRnOYz_InNGSL4uMLWQGqfrLv_8qVppUhrBxNLqS3Vujs7axZrmkibajWH=w1064-v0)

1. Layout Grid
2. Alignment

#### Keylines

Keylines are an alignment tool that enables consistent placement of elements outside of the layout grid. They are vertical lines that show where leements are placed when they don't align to the grid. Keylines are determined by each element's distance from the edge of the screen and are measured in increments of 8dp.

![keylines](https://lh3.googleusercontent.com/SrezdvoaTp-k9fPW-trPeBrnXWR3FNdQxrQWN6E0YKQlcQqQ6d6H4VNFt5r9Qzc7_3XXEdnVqQm25BX7dt9G7VqYCNZ43v6cO8JihA=w1064-v0)

1. Layout grid
2. Keyline

Keylines can create more or less space between elements in a layout. They are adjustable per breakpoint range.

## Containers and Ratios

### Containers

A container is a shape used to represent an enclosed area. Containers can hold UI elements such as images, icons, or surfaces.

![containers](https://lh3.googleusercontent.com/_jkgGGDxbyGkDUREedXaaW4gUTKAqNPvEW6whJGW3I1Rsk9qbexseRBAnktFl8qGgfG-W6sJGoOIX5ZWsocDZ-FXk8tN4rOv7spo=w1064-v0)

1. Image container
2. Icon container
3. Surface container

Containers can be rigid and restrict the size or cropping of elements within them. Alternatively, they can be flexible and grow to support the size of the content they hold.

### Aspect Ratios

An aspect ratio is the proportion of an element's width to its height. Aspect ratios are written as `width:height`.

To maintain consistency in your layout, use a consistent aspect ratio on elements like images, surfaces, and screen size.

The following aspect ratios are recommended for use across your UI: `16:9`, `3:2`, `4:3`, `1:1`, `3:4`, `2:3`.

![aspect-ratios](https://lh3.googleusercontent.com/VoBz_lg0Fh9t9YeWa4v1EvMfBqXtnXkgOKA5Wc51sU6pFDHhKkWPfrfFHPeMwtd4G4LQ5B9eSZKQNjXOsQH0gV02HpQYADd4eSK5og=w1064-v0)

### Flexible Ratios

Flexible ratio sizing is determined by the layout grid:

* Container width is determined by the screen layout and grows to fill the maximum space available.
* Container height is determined by the height of the image in the container.

Use a flexible ratio to allow content form to determine the height of the container.

Container widths are determined by the column widths in the layout grid:

![flexible-ratios](https://lh3.googleusercontent.com/uwxkWXpdEpoIPz4dUWTu3Slb17UjbDiIW2soKPiTY7JKDu0l38H1Y4JsMuIVgv7BQrz4C_HyeFQi4EdHfcTDDDMYSG9cmS6sBn-FpQ=w1064-v0)

## Responsive Cropping

To display images responsively, define how an image will be cropped at different breakpoint ranges. At different breakpoint ranges cropping can:

* Maintain one fixed ratio
* Adapt to different ratios
* Fix image heights

### Maintain One Ratio

Image sizing can hold fixed ratio across breakpoint ranges. The image in the UI maintains a `3:2` ratio between breakpoints:

![maintain-one-ratio](https://lh3.googleusercontent.com/kFP94SNxZnEdxq_IgGzVHMVEpob2wuzycwbm69Wgm1fHoPcFA19i0Cmc2votk2w9RwSYqKKVmANdvRDHfgIqaOaZfiefE3yCoEOc-wA=w1064-v0)

### Adapt to Different Ratios

Image ratios can change by adapting to different breakpoint ranges. The image ratio changes from 1:1 to 16:9 between breakpoints:

![adapt-to-different-ratios](https://lh3.googleusercontent.com/4qaK79Dr80-eHWPxi93Y2iDEby21ETywNNPPtgThZcSz5yBIw_gxUR3dz6EEZypWQeQK13l8nmnqHXRVe0-RLOjF4MSWb4Z4OEE3=w1064-v0)

### Fixed Image Heights

Image sizing can maintain a fixed height and fluid width across and within breakpoint ranges. The image maintains a fixed height while the width between breakpoints is fluid:

![fixed-image-heights](https://lh3.googleusercontent.com/lQteTxA5pZzhyyvJexW86V7XXIEK_rL3xWkS_9fKmUsZxJFDfgiDQPbFb5lDu9ATCnbMwkBWPt_XvEImxDrO8eJ4qfqFp3xNa8Ss=w1064-v0)

## Touch Targets

Touch targets apply to any device that receives both touch and non-touch input. To balance information density and usability, touch targets should be at least 48 x 48 dp with at least 8dp of space between targets:

![touch-targets](https://lh3.googleusercontent.com/zZyeNTZN0HzV8sSnlM8LA6HFDT6qtYdhOCyBzMg2t01SQZB7Vhz4ElPgWxxvHer_5l82Rz7fcq90jlzXHiTPynq8o6QAvqDNVAGYMg=w1064-v0)