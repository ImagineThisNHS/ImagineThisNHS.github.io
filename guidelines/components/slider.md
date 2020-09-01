# Slider
Sliders are used to select from a range of values.

## Examples
![example image for slider](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/slider/new%20slider%20fig.png?raw=true)

_Example of the naming and grouping for sliders_

![example image for slider](https://github.com/ImagineThisNHS/ImagineThisNHS.github.io/blob/master/guidelines/assets/slider/slider-example.png?raw=true)

_Another example of a slider group_

## Structure
A slider should be a group that contains a minimum of three text sub-components:
* Maximum value of the slider, its name containing `max_value`.
* Minimum value of the slider, its name containing `min_value`.
* Current value of the slider, its name containing `cur_value`.
All these values should be **numbers**.

Apart from these, it can also contain any graphics that are part of the slider.

## Styling
Slider currently has a default appearance on each OS, which can be easily tweaked by the developer.
```tip
Wrap a slider in a form or card to give it padding and container styling.
```

## Naming
The slider component (group) should have a name with the word `slider` contained within it + textual sub-components of `max_value`, `min_value` and `cur_value` as mentioned above.
