# Dropdown 
Dropdowns are commonly used to let a user select a single option from a list of options. 

Their native implementation on iOS and Android varies. Therefore, we implemented a completely custom dropdown that behaves consistently on both platforms and yet is close to the feel of the native ones.

## Example

Example dropdown design in Figma, alongside its structure:

![image showing dropdown ui and grouping in figma](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/dropdown/downdown%20fig%20combined.png?raw=true)

_(Left) Figma Designed Dropdown (Right) Grouping of layers_

![image showing dropdown_placeholder](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/dropdown/dropdown.png?raw=true)

_Example of Placeholder Option_

## Structure
A dropdown should be a group that contains a rectangle representing the container and a text component representing an option. (See examples above.)

## Styling
Both the rectangle and the text option can be styled and their styles should be translated into code.

## Naming
* The name of the dropdown selector's group should contain `dropdown`.
* Inside the group there should be a text element with a name containing `option`.

