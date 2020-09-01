# Background

Background elements are usually the last element within a view that covers the entire view.

## Example
The blue gradient, in the example below, shows a background element

![Image showing screenshot of figma view](https://raw.githubusercontent.com/ImagineThisNHS/ImagineThisNHS.github.io/master/guidelines/assets/background/background%20fig%201%20(50%25).png)

## Styling
Any solid color and shape will be recognised. 

This tool currently does not support gradients because their translation into React-Native is not simple and requires the use of an external package. One of the gradient colors will be used as a solid background instead.

## Naming
Background elements should be named  `background`. Additionally, the name should not contain other words such as `background 1` or `white background`.

However, the case of letters does not affect the recognition of component names; both `Background` and `background` are correct and translated into code correctly.

## Grouping
All elements and UI components should be ordered above the background element within a group. This is common sense as any elements below the background simply won't be visible even in the sketches.
