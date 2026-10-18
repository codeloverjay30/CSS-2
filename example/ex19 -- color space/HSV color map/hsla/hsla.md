# hsb()
## syntax 

With RE (Regular expression), it can be presented into

```
<hsla> := "hsla("<optionalSpaces><hueNumber><comma><saturationPercentage><comma><lightnessPercentage><comma><alpha><optionalSpaces>")"
```

where

```
<optionalSpaces> := <space>*
<spaces> := <space>+
<space> := " "
```

`<hueNumber>` indicates the hue (which also indicates the color). It should be a number between 0 and 360.

`<saturationPercentage>` indicates the saturation percentage. It should be a number between 0 and 100, followed by `%`. For example, `0%`.

`0%` means no saturation, and the color will be always be white.

`100%` means fully saturation.

`<lightnessPercentage>` indicates the lightness percentage. It should be a number between 0 and 100, followed by `%`. For example, `0%`.

`<alpha>` indicates the transparency, it should be a number between 0 and 1 (both inclusive).