# Color

## Foreground Color

The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

1. RGB values these express colors in terms of how much red, green and blue are used to make it up. For example: RGB (100, 100, and 90).

2. Hex codes these are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80.

3. Color names there are 147 predefined color names that are recognized by browsers. For example: Dark Cyan.

## Background Color

CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box. You can specify your choice of background color in the same three ways you can specify foreground colors: RGB values, hex codes, and color names (covered on the next page).

• If you do not specify a background color, then the background is transparent.

## Understanding Color

* Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.

* RGB Values for red, green, and blue are expressed as numbers between 0 and 255.

* Hex Codes Hex values represent values for red, green, and blue in hexadecimal code.

* Color Names Colors are represented by predefined names. However, they are very limited in number.

**Hue:** Hue is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue.

**Saturation:** Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray.

**Brightness:** Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark.

## Contrast

When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.

* Low Contrast: Text is harder to read when there is low contrast between background and foreground colors.

* High Contrast: Text is easier to read when there is higher contrast between background and foreground colors.

* Medium Contrast: For long spans of text, reducing the contrast a little bit improves readability.

## Opacity

CSS3 introduces the opacity property which allows you to specify the opacity of an element and any of its child elements. The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).

## CSS3: HSL Colors

CSS3 introduces an entirely new and intuitive way to specify colors using hue, saturation, and lightness values.

**Hue:** Hue is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360.

**Saturation:** Saturation is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.

**Lightness:** Lightness is the amount of white (lightness) or black (darkness) in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as luminosity.

## Notes

1. Color not only brings your site to life, but also helps convey the mood and evokes reactions.

2. There are three ways to specify colors in CSS: RGB values, hex codes, and color names.

3. Color pickers can help you find the color you want.

4. It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).

5. CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.

6. CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.
