# Designing for Imagine This

This tool can take a Figma UI design prototype and generate the code required for a functional React Native Application. There is some key consideration when designing the UI within Figma. This section helps further elaborate this and describe how to organise UI elements to allow for optimal code conversion.

## How Imagine This Works
Here is a basic overview of how the Imagine This tool works. This will help explain some basic inner workings of the project, which will help further demonstrate how these guidelines assist the constraints of the problem.

1. Figma file’s contents are read via the Figma API
2. The user selects the view that they would like to be converted into React Native Code
3. For each of the selected views, all layers are traversed by the tool
4. Each layer’s name, attributes (size, border, shape, etc.) are used to determine the UI element
5. A React Native App source code will be generated from the Figma sketch. The output will be in the form of a zip, with files in their correponding position in the application folder.

## Naming Scheme

```warning
When you create an app with multiple pages, you need to make sure each page has a **unique name**. Also, please do not call your pages any of the following: SafeAreaView, Image, React or NavigationContainer. Doing so would make your app fail to compile due to JS import clashes.
```

Based on the description of how the system works, one of the core methods of identifying a UI component is through its name. For example, a **text input field** should include **“input”** within its name (for example “phone input”), a **dropdown selector** should contain **“Dropdown”**, etc. Apart from assisting us in component recognition, following these naming conventions and file structure in Figma will ensure **good document readability** and will enable reuse of components. It is considered good design practice and will be appreciated by any fellow designer who inherits the Figma project.

To get the most out of the Imagine This tool, we strongly recommend reading about our **recommended naming conventions** in the **'Components'** section. If these conventions are not followed, this tool will still attempt to recognise UI elements and generetate their code, however, the more specific and complicated UI elements may not be recognised fully and correctly and the generated code will be incomplete.
