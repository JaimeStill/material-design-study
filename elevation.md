# Elevation

Re-visit the notion of elevation in the UI. Foundational layout principles apply to all Material elements, and we need to consider that these elements are layered within a three-dimensional space. Consider the root layer as the surface of a desk. Everything past that point is then placed at layers above that surface. Elements can be placed above other elements, creation tertiary and beyond layers.

I think this is where the flat design starts to lose its impact (and the replication of borders descends into line recursive hell). It seems that the biggest thing about implementing elevation that was perhaps making it not feel right when initially used was a lack of subtlety. The resting elevations, as well as their resulting dynamic elevation offsets, should be less severe than they were when implemented previously.

> Read about the design team's [research wiht low-vision participants](https://material.io/design/environment/light-shadows.html#research) illustrating how shadows and outlines impact an individual's ability to identify and interact with a component.

[Per the Material spec](https://material.io/design/environment/elevation.html#elevation-in-material-design):

> Resting elevations on desktop are shallower because other cues, like hover states, communicate when a component is interactive. For example, cards at 0dp elevation on desktop are outlined with a stroke.

**Desktop Resting Elevation**  

![desktop-resting-elevation](https://lh3.googleusercontent.com/lg7Rz0Ji-yv2fpd1wo7SRkWvseJEmBndg0vicbmF6N6OW_D7YPGeQOIxzfIs8anpg5umfzCfLSPMikyEZUvjt5WOrFwD60AgyIxMAg=w1064-v0)

**Desktop Dynamic Elevation Offset**

![desktop-dynamic-elevation-offset](https://lh3.googleusercontent.com/IGup0QloUkkozMfTPbOYOCjUZrfaeNUMLKRBJ6fLBgSUj0_WnzNNy1GsyUijEJyEqDYGqbEW1G3UFO3XOLdZcfd278WCK01TWMOlWQ=w1064-v0)

Stroke in this context should be used to indicate resting elements that are not currently the focus of interaction. This concept can also be a good extension point for the glow feature, the idea being that a resting element can have a stroke of a given color. When that element is in an interactive state of elevation, it would be elevated with a glow-based shadow corresponding to its stroke color.

Dynamic elevation offsets are default elevations components move to in response to user input or system events. They are the same across each type of component. Once the triggering event is copmlete, the component should swiftly return to its resting elevation.

## Default Elevations

Component | Default Elevation Values (px)
----------|------------------------------
Dialog | 24
Modal Bottom / Side Sheet | 16
Navigation Drawer | 16
Floating Action Button - Pressed | 12
Standard Bottom / Side Sheet | 8
Bottom Navigation Bar | 8
Bottom App Bar | 8
Menus and Sub-Menus | 8
Card (when picked up) | 8
Contained Button (pressed state) | 8
Floating Action Button - Resting | 6
Snackbar | 6
Top App Bar (scrolled state) | 4
Top App Bar - Resting | 0 or 4
Refresh Indicator Search Bar (scrolled state) | 3
Contained Button (resting elevation) | 2
Search Bar (resting elevation) | 1
Card (resting elevation) | 1
Switch | 1
Text Button | 0
Standard Side Sheet | 0

![default-elevation-values](https://lh3.googleusercontent.com/pEk_CLv7V6MroLmKY5rA5nCknpKI0ltFZn5yypHiAt0zJzWd5frkMaj2VXWpQmcPtoA_8P-2n0wg9I4JgCWSOKN5nUSgN7IActWvZw=w1064-v0)

## Implementation Tasks

In the **Motion and elevation** section of [Depicting Elevation](https://material.io/design/environment/elevation.html#depicting-elevation), there are strategies for transitioning focus using elevation. These patterns would be very useful for working with elements. Their implementation would drastically improve the fluidity of our apps without impacting performance (as this motion is handled natively by the browser and incurs no penalties as a result of network latency).

