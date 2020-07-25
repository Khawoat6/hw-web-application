# Chapter 5: Themes, Colors, and Polish

## Table Content

[Introduction](#Introduction)

- [The Markup](#The-Markup)
- [Inverting Colors](#Inverting-Colors)
- [New HTML Elements in the Theme](#New-HTML-Elements-in-the-Theme)
- [New CSS Background Properties](#New-CSS-Background-Properties)
- [Exercise 5.01: Creating a Dark Theme](#Exercise-5.01:-Creating-a-Dark-Theme)
- [Creating a Dark Theme with the HSL Function](#Creating-a-Dark-Theme-with-the-HSL-Function)
- [Exercise 5.02: Creating a Dark Theme Using hsl](#Exercise-5.02:-Creating-a-Dark-Theme-Using-hsl)
- [CSS Invert Filter](#CSS-Invert-Filter)
- [Exercise 5.03: Creating a Dark Theme with the CSS Invert Filter](#Exercise-5.03:-Creating-a-Dark-Theme-with-the-CSS-Invert-Filter)
- [CSS Hooks](#CSS-Hooks)
- [Exercise 5.04: Customizing a Theme with CSS Hooks](#Exercise-5.04:-Customizing-a-Theme-with-CSS-Hooks)
- [Activity 5.01: Creating Your Own Theme Using a New Color Palette](#Activity-5.01:-Creating-Your-Own-Theme-Using-a-New-Color-Palette)

[Summary](#Summary)

## Introduction

### The Markup

![Getting Started](images/img1.png)

### Inverting Colors

```link
https://www.colortools.net/color_complementary.html
```

### New HTML Elements in the Theme

- `pre` (preformatted element)
- `abbr` (abbreviation element)

### New CSS Background Properties

- `background-image`
- `background-repeat`
  - `repeat`
  - `space`
  - `round`
  - `no-repeat`

### _Exercise 5.01: Creating a Dark Theme_

![Getting Started](images/ex5-01.png)

### Creating a Dark Theme with the HSL Function

The HSL function allows you to update the color value of a property by using one of three arguments: **H**ue, **S**aturation, or **L**ightness:

- `H` represents the hue as an angle on the color wheel. You can specify this using degrees (or, programmatically, radians.) When provided as a unitless number, it is interpreted as degrees, with 0 as pure red, 120 as pure green, and 240 as pure blue.
- `S` represents the saturation, with 100% saturation being completely saturated, while 0% is completely unsaturated (gray). 50% is a "normal" color.
- `L` represents the saturation, with 100% saturation being completely saturated, while 0% is completely unsaturated (gray).

  ![Getting Started](images/img2.png)

### _Exercise 5.02: Creating a Dark Theme Using hsl_

![Getting Started](images/ex5-02.png)

### CSS Invert Filter

`filter: invert().`

![Getting Started](images/img3.png)

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <title>Invert Filter</title>
    <style type="text/css">
      .invert {
        filter: invert(100%);
      }
    </style>
  </head>
  <body>
    <p>
      <img
        src="./assets/react-2019-7.jpg"
        width="100%"
        alt="a mural by the author"
      />
    </p>
    <p>
      <img
        src="./assets/react-2019-7.jpg"
        width="100%"
        alt="a mural by the author"
        class="invert"
      />
    </p>
  </body>
</html>
```

### _Exercise 5.03: Creating a Dark Theme with the CSS Invert Filter_

![Getting Started](images/ex5-03.png)

### CSS Hooks

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
    <title>Using CSS hooks</title>
    <style type="text/css">
      .tag-css {
        background: #003366;
      }
      .tag-html {
        background: #006600;
      }
      .tag-javascript {
        background: #660000;
      }
    </style>
  </head>
  <body class="tag-css"></body>
</html>
```

### _Exercise 5.04: Customizing a Theme with CSS Hooks_

![Getting Started](images/ex5-04.png)

### _Activity 5.01: Creating Your Own Theme Using a New Color Palette_

## Summary

<!-- CONTACT -->

## Contact

Oat Phattaraphon - [@phattaraphon_c](https://twitter.com/phattaraphon_c)
