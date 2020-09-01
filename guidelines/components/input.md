# Input field
Input fields allow users to enter user input. Typically they are used within forms, search boxes, to send messages and more.

## Example

_Example of an input field_

![Example screenshot of textbox layers and group](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/textbox/textbox%20fig.png?raw=true)

## Structure
* An input field should be a group that contains a Rectangle that represents its container.
* (Optional) Can contain Text representing a **label**.
* (Optional) Can contain Text representing a **placeholder**.

_Example of Input structure_

![Example label placeholder](https://github.com/ImagineThisUCL/ImagineThisUCL.github.io/blob/master/guidelines/assets/textbox/input-structure.png?raw=true)

## Styling
* Any styles of the container (Rectangle), such as background, border, corner radius, etc. will be translated into code.
* Any text styles applied to the optional label and placeholder will be also translated into code.

## Naming and Grouping
* All the elements within the input component should be contained within a group with a name that contains `input`.
* Label text should contain the word `label` in its name.
* Placeholder text should contain the word `placeholder` in its name.

_Example of How Label and Placeholder looks on the frontend_

![Example label placeholder](https://github.com/ImagineThisUCL/ImagineThisUCL.github.io/blob/master/guidelines/assets/textbox/label&&placeholder.png?raw=true)

