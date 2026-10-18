# lch()
## syntax 

+ basic syntax

With RE (Regular expression), it can be presented into

```
<lch> := "lch("<optionalSpaces><lightnessPercentage><spaces><chromaNumber><spaces><hueNumber><optionalSpaces>")"
```

where

```
<optionalSpaces> := <space>*
<spaces> := <space>+
<space> := " "
```

`<hueNumber>` indicates the hue (which also indicates the color). It should be a number between 0 and 360.

`chromaNumber` indicates the [chroma](https://en.wikipedia.org/wiki/Colorfulness). It should be a number between 0 and 100.

`<lightnessPercentage>` indicates the lightness percentage. It should be a number between 0 and 100, followed by `%`. For example, `0%`.

+ other similar syntax

```
<lch> := "lch("<optionalSpaces><lightnessPercentage><spaces><chromaPercentage><spaces><hueNumber><optionalSpaces>")"
```

`<chromaPercentage>` indicates the [chroma](https://en.wikipedia.org/wiki/Colorfulness) percentage. It should be a number between 0 and 100, followed by `%`.

For other similar syntax, see [`lch()`](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/lch)

+ advanced syntax

```
<lch> := "lch("<optionalSpaces><lightnessPercentage><spaces><chromaNumber><spaces><hueNumber><spaces>"/"<alphaPercentage><optionalSpaces>")"

```

where

`<optionalSpaces>` and `<spaces>` are defined in above section.

`<alphaPercentage>` indicates the transparency, it should be a number between 0 and 100 (both inclusive), followed by `%`. (For example, `20%`)

> [!WARNING]
> The advanced syntax of `hwb()`
> 
> ```
> <hwb> := "hwb("<optionalSpaces><hueNumber><spaces><saturationPercentage><spaces><brightnessPercentage><optionalSpaces>")"
> ```
> 
> is only supported on new platform.
>
> As a developer, if you want to develop it for older version of web browser, please consider the other approach.

> [!WARNING]
> There are no `hwba()` function in native CSS. 