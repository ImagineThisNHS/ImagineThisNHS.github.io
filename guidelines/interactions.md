# Interactions

A powerful feature of modern design prototype software is creating links and interactions. For instance, a link can be created between a button and a wireframe. When the button is clicked/tapped, it will navigate to the linked wireframe. This provides rich interactions that can visually and interactively demonstrate how the final app would function during the prototyping phase. This is commonly used within Figma prototype design.

This tool can read pre-defined interactions (mostly transition between wireframes) within the Figma prototype and converts them into actual redirect links between app pages in the generated React-Native App. 

```warning
Currently, only `onTap` interactions within Figma are supported. `onTap` is a default interaction option.
```

## Interaction Types
Currently, the Imagine This tool only supports `On Tap` interactions. Other interactions are ignored and will not be translated into code.

## Design Logic (one button-one page)
Concerning to the logic part, currently the design sketch should follow the rule of "one button corresponding to one wireframe". If you have a common navigation bar in the app, please make sure that each of the buttons within only links to one and only one wireframe. Any exception may leads to logic errors with the link missing or incomplete code generation.

## Animations
Custom animations for interactions are not yet supported. For all animations, we use the default behaviour for iOS and Android. For instance, a modal view within iOS has a default animation of sliding up from the bottom.
