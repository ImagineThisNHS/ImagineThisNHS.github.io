# Map

Maps are another of the more dynamic elements inside UI design. All maps designed in Figma are simply mockups and it would be pointless to try to derive any data from them. Therefore, we treat maps as mockups in the code generation as well, and simply output a map module that can be easily customised and extended by the developer.

## Example

_Example of a Map placeholder in Figma_

![image showing chart ui and grouping in figma](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/map/map.png?raw=true)

## Structure
Our tool currently outputs a map module in place of any map that it finds in the wireframes. There is no specific structure requirement.

```warning
Any elements/components that are placed on top of the map in the Figma file will be rendered in a lower position underneath the map within the code and left for the developer to connect and overlay.
```

## Styling
No styles can be applied to the map - Google/Apple maps are used.

## Naming
* The map may be a rectangle or an image and its name should contain `map`.
