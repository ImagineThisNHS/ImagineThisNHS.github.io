# Button

```note
Buttons are divided into **text button** and **image button**.
```

## Text Button
### Examples
![text button example images](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/button/text%20button.png?raw=true)

![text button example images](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/button/circle%20button.png?raw=true)

_Examples of Text Button Apperance_

### Styling
A Figma element composed of a _shape (rectangle or circle)_ and _text_.

### Naming & Grouping
* The text button should be a group.
* The group name should contain the word `textbutton`.
* Besides text, the groups are also required to contain a rectangle or a cricle (we only support these two shapes right now).


## Image Button
### Examples
![image button examples images](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/button/image%20button.png?raw=true)

_Examples of Image Button Apperance_

### Styling
A Figma element composed of _graphics (or group of shapes)_ without text.

### Naming & Grouping
* The image button should be a group.
* The group name should contain the word `imagebutton`.
* The image button group should have a sub-component with its name containing one of the words `image`, `icon` or `picture`, this component will be downloaded as the image.

```tip
The image sub-component can be a single bitmap/vector image or even a group of any other elements (such as multiple vectors that collectively form an image). In the latter case, this tool will download and render the entire group as a bitmap.
```
