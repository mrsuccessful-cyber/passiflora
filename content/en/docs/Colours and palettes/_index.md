
---
title: "Colours and Palettes"
linkTitle: "Colours and Palettes"
weight: 4
date: 2017-01-05
simple-list: true
description: >
  A total of sixteen, carefully selected, dimmed pastel colours for a eye-comfortable, but yet colourful ambiance.
---
![](undraw_palette.svg)

The Rosely base colours consists of four named colour palettes providing different syntactic meanings and colour effects for dark & bright ambiance designs. These colours are specifically chosen to complement each other as well as a warmer and more colourful alternative to the Nord colour palette, so can be used for code syntax highlighting and UI components.

It has been created for **clear, uncluttered and elegant designs** following a **minimal and flat** style pattern.
For syntax highlighting it aims to ensure an **undisturbed focus on important parts of the code**, a **good readability** and a **quick visual distinction** between the different syntax elements.

All colours are numbered from `rosely0` to `rosely15` where each palette contains a different amount of colours. The naming convention preserves the compatibility for terminal colour schemes and allows an uncomplicated use as base for such.

This document provides a set of guidelines detailing how to style and highlight code syntax and UI elements.
Please note that these guidelines are “soft“ recommendations to describe the original idea of Rosely!
They may be used in a modified form like e.g. different use cases for a specific colour or with different shading options applied.

## Velvet Night

{{< swatch-group name="Velvet Night" >}}
{{< swatch color="#27272a" code="rosely0" name="Black Beauty" pantone="19-3911 TCX" >}}
{{< swatch color="#615f5f" code="rosely1" name="Granite Gray" pantone="18-5204 TCX" >}}
{{< swatch color="#85677b" code="rosely2" name="Grapeade" pantone="18-3211 TCX" >}}
{{< swatch color="#a49e9e" code="rosely3" name="Opal Gray" pantone="16-3801 TCX" >}}
{{< /swatch-group >}}

**Velvet Night** is made up of four darker colours that are commonly used for base elements like backgrounds or text colour in _bright ambiance designs_.

### `rosely0`

**An intense black.**

For _dark ambiance designs_, it is used for background and area colouring while not being used for syntax highlighting at all because otherwise it would collide with the same background colour.

For _bright ambiance designs_, it is used for base elements like plain text, the text editor caret and reserved syntax characters like curly- and square brackets.
It is rarely used for passive UI elements like borders, but might be possible to achieve a higher contrast and better visual distinction (harder/not flat) between larger components.

### `rosely1`

**A dark grey.**

For _dark ambiance designs_ it is used for elevated, more prominent or focused UI elements like

- status bars and text editor gutters
- panels, modals and floating popups like notifications or auto completion
- user interaction/form components like buttons, text/select fields or checkboxes

It also works fine for more inconspicuous and passive elements like borders or as dropshadow between different components.
There's currently no official port project that makes use of it for syntax highlighting.

For _bright ambiance designs_, it is used for more subtle/inconspicuous UI text elements that do not need so much visual attention.
Other use cases are also state animations like a more brighter text colour when a button is hovered, active or focused.

### `rosely2`

**A dark purplish colour.**

For _dark ambiance designs_, it is used to colourize the currently active text editor line as well as selection- and text highlighting colour.
For both _bright & dark ambiance designs_ it can also be used as an brighter variant for the same target elements like `rosely1`.

### `rosely3`

**A medium gray colour.**

For _dark ambiance designs_, it is used for UI elements like indent- and wrap guide marker.
In the context of code syntax highlighting it is used for comments and invisible/non-printable characters.

For _bright ambiance designs_, it is, next to `rosely1` and `rosely2` as darker variants, also used for the most subtle/inconspicuous UI text elements that do not need so much visual attention.

## Spring Blossom

{{< swatch-group name="Spring Blossom" >}}
{{< swatch color="#f7caca" code="rosely4" name="Milennial Pink" pantone="13-1520 TCX" >}}
{{< swatch color="#f4dede" code="rosely5" name="Heavenly Pink" pantone="12-1305 TCX" >}}
{{< swatch color="#f4eee8" code="rosely6" name="Sugar Swizzle" pantone="11-0607 TCX" >}}
{{< /swatch-group >}}

**Spring Blossom** is made up of three bright colours that are commonly used for text colours or base UI elements in _bright ambiance designs_.

The palette can be used for two different shading ambiance styles:

- bright to dark — This is the **recommended style** that uses `rosely6` as base colour and highlights other UI elements with `rosely5` and `rosely4`.
- dark to bright (_semi-light_) — This style uses `rosely4` as base colour and highlights other UI elements with `rosely5` and `rosely6`.

The documentation of the different colours from this palette are based on the recommended _bright to dark_ ambiance style.
To apply the colour purposes to the _dark to bright_ style the definitions can be used in reversed order.

### `rosely4`

**The base colour for Rosely, a warm and embracing gentle rose tone that conveys compassion and a sense of composure.**

For _dark ambiance designs_, it is used for UI elements like the text editor caret.
In the context of syntax highlighting it is used as text colour for variables, constants, attributes and fields.

For _bright ambiance designs_, it is used for elevated, more prominent or focused UI elements like

- status bars and text editor gutters
- panels, modals and floating popups like notifications or auto completion
- user interaction/form components like buttons, text/select fields or checkboxes

It also works fine for more inconspicuous and passive elements like borders or as dropshadow between different components.
In the context of syntax highlighting it is not used at all.

### `rosely5`

**A very light shade of pink, a colour tempering passion with purity. It is the lighter, most gentle, blissful and acquiescent of the red family, and elicits an aura of innocent romance**

For _dark ambiance designs_, it is used for more subtle/inconspicuous UI text elements that do not need so much visual attention.
Other use cases are also state animations like a more brighter text colour when a button is hovered, active or focused.

For _bright ambiance designs_, it is used to colourize the currently active text editor line as well as selection- and text highlighting colour.

### `rosely6`

**A sugary white.**

For _dark ambiance designs_, it is used for elevated UI text elements that require more visual attention.
In the context of syntax highlighting it is used as text colour for plain text as well as reserved and structuring syntax characters like curly- and square brackets.

For _bright ambiance designs_, it is used as background and area colouring while not being used for syntax highlighting at all because otherwise it would collide with the same background colour.

## Forest Meadow

{{< swatch-group name="Forest Meadow" >}}
{{< swatch color="#93a9d1" code="rosely7" name="Karuna Blue" pantone="15-3919 TCX" >}}
{{< swatch color="#be9cc1" code="rosely8" name="Lupine" pantone="16-3521 TCX" >}}
{{< swatch color="#b0879b" code="rosely9" name="Orchid Haze" pantone="16-2107 TCX" >}}
{{< swatch color="#b565a7" code="rosely10" name="Radiant Orchid" pantone="18-3224 TCX" >}}
{{< /swatch-group >}}

**Forest Meadow** can be described as the accent palette of Rosely, a group of four bluish/purplish colours that are commonly used for primary UI component and text highlighting and essential code syntax elements.

All colours of this palette are used the same for both _dark & bright ambiance designs_.

### `rosely7`

**A cool and tranquil blue colour comforts with a calming effect.**

Used for UI elements that should, next to the primary accent colour `rosely8`, stand out and get more visual attention.
In the context of syntax highlighting it is used for classes, types and primitives.

### `rosely8`

**A light colour reminiscent of a field of sundial lupines, bringing back memories of Lake Tekapo in New Zealand.**

Used for primary UI elements with main usage purposes that require the most visual attention.
In the context of syntax highlighting it is used for declarations, calls and execution statements of functions, methods and routines.

### `rosely9`

**A slightly warm-toned, medium lavender, recalling the heady scents of a tropical garden.**

Used for secondary UI elements that also require more visual attention than other elements.
In the context of syntax highlighting it is used for language specific, syntactic and reserved keywords as well as

- support characters
- operators
- tags
- units
- punctuations like (semi)colons, points and commas

### `rosely10`

**A captivating harmony of fuchsia, purple and pink undertones, this colour emanates great joy, love and health.**

Used for tertiary UI elements that require more visual attention than default elements.
In the context of syntax highlighting it is used for pragmas, comment keywords and pre-processor statements.

## Vivid Floriade

{{< swatch-group name="Vivid Floriade" >}}
{{< swatch color="#d2386c" code="rosely11" name="Raspberry Sorbet" pantone="18-2043 TCX" >}}
{{< swatch color="#ec809e" code="rosely12" name="Morning Glory" pantone="15-1920 TCX" >}}
{{< swatch color="#eada4f" code="rosely13" name="Meadowlark" pantone="13-0646 TCX" >}}
{{< swatch color="#64bfa4" code="rosely14" name="Spearmint" pantone="15-5819 TCX" >}}
{{< swatch color="#919bc9" code="rosely15" name="Easter Egg" pantone="16-3925 TCX" >}}
{{< /swatch-group >}}

**Vivid Floriade** consists of five colourful components reminiscent of Canberra's annual flower festival.

All colours of this palette are used the same for both _dark & bright ambiance designs_.

### `rosely11`

**A delectable raspberry colour.**

Used for UI elements that are rendering error states like linter markers and the highlighting of Git `diff` deletions.
In the context of syntax highlighting it is used to override the highlighting of syntax elements that are detected as errors.

### `rosely12`

**A bold hot pink.**

Rarely used for UI elements, but it may indicate a more advanced or dangerous functionality.
In the context of syntax highlighting it is used for special syntax elements like annotations and decorators.

### `rosely13`

**A vibrant sunny yellow.**

Used for UI elements that are rendering warning states like linter markers and the highlighting of Git `diff` modifications.
In the context of syntax highlighting it is used to override the highlighting of syntax elements that are detected as warnings as well as escape characters and within regular expressions.

### `rosely14`

**A muted green bringing memories of a herb garden.**

Used for UI elements that are rendering success states and visualizations and the highlighting of Git `diff` additions.
In the context of syntax highlighting it is used as main colour for strings of any type like double/single quoted or interpolated.

### `rosely15`

**A soft blue reminiscent of Easter eggs.**

Rarely used for UI elements, but it may indicate a more uncommon functionality.
In the context of syntax highlighting it is used as main colour for numbers of any type like integers and floating point numbers.
