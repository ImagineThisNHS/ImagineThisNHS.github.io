# Designing for Imagine This

This tool can take a Figma UI design and generate the code required for a React Native Application. There is some key consideration when designing the UI within Figma. This section helps further elaborate this and describe how to organise UI elements to allow for optimal code conversion.

## How Imagine This Works
Here is a basic overview of how the Imagine This tool works. This will help explain some basic inner workings of the project, which will help further demonstrated how these guidelines assist the constraints of the problem.

1. Figma file’s contents are read via the Figma API
2. The user selects the view that they would like to be converted into React Native Code
3. For each of the selected views, all layers are traversed by the tool
4. Each layer’s name, attributes (size, border, shape, etc.) are used to determine the UI element

## Naming Scheme
Based on the description of how the system works, the core method of identifying a UI component is through its name. For example, a text input field should include “Text Box” within its name, and a dropdown selector should be named as “Dropdown”. This will produce the optimal recognition since the name of the corresponding elements largely determines UI components. If these rules are not followed, some design UI elements may not be recognised correctly. Furthermore, the corresponding code may not be generated successfully.
