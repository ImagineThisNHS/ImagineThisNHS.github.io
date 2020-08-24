# Interactions

A powerful feature of modern design prototype software is creating links and interactions. For instance, a link can be created between a button and a view. When the button is clicked/tapped, it will navigate to the linked view. This provides rich interactions that can visually and interactively demonstrate how the final app would function during the prototyping phase. This is commonly used within Figma prototype design.

This tool can read defined interactions within the Figma prototype and converts them into transitions between views in the generated React-Native App. In more technical terms, it generates a Navigation Stack for the application from these interactions.

```warning
Currently, only `onTap` interactions within Figma are supported.
```

## Limitations
### Interaction Types
Currently, the Imagine This tool only supports `On Tap` interactions. Other interactions are ignored and not translated into code.

### Animations
Custom animations for interactions are not yet supported. For all animations, we use the default behaviour for iOS and Android. For instance, a modal view within iOS has a default animation of sliding up from the bottom.
