# CSS properties: Text

## Color

### Documentation

|Website  |URL                                                   |
|---------|------------------------------------------------------|
|CSSWG    |https://drafts.csswg.org/css2/#propdef-color          |
|W3CSchool|https://www.w3schools.com/cssref/pr_text_color.php    |
|MDN      |https://developer.mozilla.org/en-US/docs/Web/CSS/color|

### Codename

```
color
```

### Value

```
<color> | inherit
```

[Color units](https://drafts.csswg.org/css2/#color-units)

### Description

Color of the text.

The color CSS property sets the foreground color value of an element's text and text decorations, and sets the `currentColor` value. `currentColor` may be used as an indirect value on other properties and is the default for other color properties, such as border-color.

### Examples

```css
/* Keyword values */
color: currentColor;

/* <named-color> values */
color: red;
color: orange;
color: tan;
color: rebeccapurple;

/* <hex-color> values */
color: #090;
color: #009900;
color: #090a;
color: #009900aa;

/* <rgb()> values and legacy <rgba()> values*/
color: rgb(34, 12, 64);
color: rgb(34, 12, 64, 0.6);
color: rgba(34, 12, 64, 0.6);
color: rgb(34 12 64 / 0.6);
color: rgba(34 12 64 / 0.6);
color: rgb(34.6 12 64 / 60%);
color: rgba(34.6 12 64 / 60%);

/* <hsl()> values and legacy <hsla()> values */
color: hsl(30, 100%, 50%);
color: hsl(30, 100%, 50%, 0.6);
color: hsla(30, 100%, 50%, 0.6);
color: hsl(30 100% 50% / 0.6);
color: hsla(30 100% 50% / 0.6);
color: hsl(30.2 100% 50% / 60%);
color: hsla(30.2 100% 50% / 60%);

/* <hwb()> values */
color: hwb(90 10% 10%);
color: hwb(90 10% 10% / 0.5);
color: hwb(90deg 10% 10%);
color: hwb(1.5708rad 60% 0%);
color: hwb(0.25turn 0% 40% / 50%);

/* Global values */
color: inherit;
color: initial;
color: revert;
color: revert-layer;
color: unset;
```

**Samples**:
* [Basic](../../../example/properties/color/color.html)
