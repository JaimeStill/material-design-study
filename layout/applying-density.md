# Applying Density

Material Design offers guidance on high-density spacing for use cases where increased density improves the user experience.

## Principles

### Scannable

![scannable](https://lh3.googleusercontent.com/PS3YYWdPb4GG-jV_1Omar8bu3KkDhDGGiB0b_yth-n4taDoQHaUhJ4P1jaGB1y56QknLvJroA3LECfD4fSYlJaRSYSN_vl2OE2SNdXQ=w1064-v0)

Dense UIs improve the ease of viewing and navigating large amounts of content.

### Prioritized

![prioritized](https://lh3.googleusercontent.com/XISmrp_WnOuollXxWA7Rkx_UvaSRNt339n4PeraoFfYc-vD0lax5jnfrvbI6FSfuRGJvw4dOliSIFOZ0BT8MbIcuEAPJnIualCxs7w=w1064-v0)

Dense UIs help users focus by reducing the space between actions.

### Visible

![visible](https://lh3.googleusercontent.com/u3kDY7X_vbyHZbEo_2aWlCkt0y2d9K6fDxgSSB0cly22RB8yLWsI-wiGyZPmZFXgL48jC8UWToHlXNTCY4HA5_qtXkbPgBeuPvXs=w1064-v0)

Increasing density allows more content and actions to fit on a single screen.

## Density Guidelines

How users interact with a component should determine whether or not you increase the density in a UI. When users view and interact with large amounts of information, high density components can improve the experience.

By making more content available on-screen, increasing the density of lists, tables, and long forms makes information easier to scan, view, and compare.

![increasing-density](https://lh3.googleusercontent.com/gkWItWB25nEUuBKZ-VQN2QLnDWtg03lUdt9betFW1BuX3WR1OCbWddxt1t80WHA9FcxW2Evc4yV_j_Yx3QsJbcBqsjM5NxE4m0sM=w1064-v0)

1. Increasing the density of a data table
2. Increasing the density of a form

### When Not to Apply Density

Tasks and alert-based components should not increase density.

#### Focused Tasks

Don't increase the density of components that involve focused tasks, such as interacting with a dropdown menu or picker. Increasing density on components such as date pickers reduces usability by limiting tappable space.

#### Alerts and Messaging

Don't increase the density in components that alert the user of changes, such as snackbars or dialogs. Increasing the density of alerts makes them less effective at attracting user attention. In the example of dialogs, readability and prominence of a message are compromised when density increases.

## Layout

### Grid and Component Density

Maintain balance between component density and grid layout.

To create scannable groups of content, use a less-dense grid layout in combination with high-density components. The denser your components become, the larger the margins and gutter widths should be. Combining a dense layout grid with dense components can make differentiating groups of content harder for users.

Do: Components with greater density should have lower density margins and gutters:

![dense-content-with-space](https://lh3.googleusercontent.com/6B3dr5mN9u8dtgBtVGgLpDcXclip0KOjZzLfSWXhPiGQNF_v2nq2HK5iNxqr4visWHx23Ewwx7oC81v9YpH8IBd-xOkAsr7QUsuTCA=w1064-v0)

Don't use a dense layout grid with dense components:

![dense-content-without-space](https://lh3.googleusercontent.com/lzjCGd26Fu36Bp1JPp0FW-RMmyd9PB4QLLsNCwnUKc_AYmFbJFXcSBZqo3ulygZ4b0bTAOuwJskEmHsy9G30a8pQg2Ogc5uyUsAtvCY=w1064-v0)

## Components

### Applying Density to Components

Component density should not be adjusted in isolation. Instead, apply density consistently to create a cohesive component set. When you adjust one component's density, consider how that change will affect other components in your app.

### Density Scale

The density scale allows you to control the density of individual components when needed.

The density scale is numbered, starting at 0 for a component's default density. The scale moves to negative numbers (-1, -2, -3) as space decreases, creating higher density. Each increment represents a decrease in the height of a component by 4dps.

The density scale applied to a button:

![button-density-scale](https://lh3.googleusercontent.com/tGIiM1A050en8x0jKvbddKzuCHsJfBBbbIFiXgB6dZvvpXKCXeEotVd2V25CVFMSmmC3MI5hEkeFo4hVzMmGDm_v37TlkNuFJWSMpA=w1064-v0)

Don't select a number from the density scale that breaks your component. The density of a chip at -4 breaks the component:

![broken-chip-density-scale](https://lh3.googleusercontent.com/uF_xm_ekRWFoT0_LMN_IEREkimLzFcxY6dUAwS4KuqBoJKCEYjeAd3R39KUojDrFK3O10NNText1KW2Bt45sc5tVIjnXHaf-B3M15A=w1064-v0)

### Spacing Methods

When a component's density increases, the padding and alignment remains consitent, but the dimension changes.

#### Padding

![padding-density](https://lh3.googleusercontent.com/Ul7L6te2ymUJA44e1pc7OiXMQzxnjukLaOobq7Mpp63SksVMvZOuhcCQIqdSlJVn2rOj9sOSnYvWYLaYK1nQ3chMAnpGWTC23oZR=w1064-v0)

Do not change the padding of a component when increasing its density. Component padding affects height and reducing padding can affect user interactions negatively.

#### Dimensions

![dimensions-density](https://lh3.googleusercontent.com/Ox6J6d6F42BQ-GlsFObzYBN9F7f65tRCdtAw5sxnZHpuDra0HEiD2lYnyMeJt8gkmFAxXYOunyitore_JPH0dUoW6MjaKJ1iGF8B_A=w1064-v0)

Change dimensions when increasing the density of components. Component dimensions affect the length and height of the component or element.

#### Alignment

![alignment-density](https://lh3.googleusercontent.com/mIqC8pzhQbGiXx9FW1oZ481sMwdMrRhvHH6gIR6b1Q9eZunikCWMaAOJzDHaWE6qWBeDTDReLAAYD2iYZS-DG19oLEBvSTTYYfIbQAQ=w1064-v0)

Use a center specification to align elements within component containers. Center aligning elements allows component heights to be adjusted without additional alignment of elements.

## Accessibility

### Touch Targets

Touch targets apply to any device that receives both touch and non-touch input. To balance information density and usability, the touch target for default density components should be at least 48 x 48 db, with at least 8dp of space between each target.

![touch-targets](https://lh3.googleusercontent.com/V4b7XLQEDBFUYzW8euExHdTcg4WljiiOBATYi4b4zpPrfOaNiDsI-K6PtLuLprHF57QmSyEUlnfk2nNbZhc3u3xCwNH44LVJ-j0SnHU=w1064-v0)

Touch target minimum of 48 x 48 dp  
1. 40dp element, 48dp touch target
2. 24dp element, 48dp touch target
3. 36dp element, 48dp touch target

A pattern for users to opt into a denser component experience:

![density-setting](https://lh3.googleusercontent.com/7vgBb31tgNlrd9jUFJbfvi4SQ_0rhiyV_9LwyN_z2WRzwGutSausk2oT5ugtrWF-BMo8XB8yf8fZWJA-SAwv-tTzpVpbUEBF36rR=w1064-v0)

## Typography

### Line Height

Line height is the space between lines of text. Line height can be used as a way to create density in typographic layouts.

![line-height-density](https://lh3.googleusercontent.com/JauXlbrLtzg79pwiytvDchPnQ6DNPsYMrAxudq4PpdOTzHUho2a85Btxmp-e_DJKTDodXGx0doDyEr4DDpgUMAi6k-kLPCXvCn5LurM=w1064-v0)

1. Larger line height: 44dp, 40dp, 44dp, 32dp
2. Smaller line height: 36dp, 32dp, 40dp, 20dp

## Implementation

Density support is currently [available for the Web platform](https://material.io/develop/web/components/density/).