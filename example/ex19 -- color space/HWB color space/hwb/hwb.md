# hsb()
## syntax 

+ basic syntax

With RE (Regular expression), it can be presented into

```
<hwb> := "hwb("<optionalSpaces><hueNumber><spaces><whitenessPercentage><spaces><brightnessPercentage><optionalSpaces>")"
```

where

```
<optionalSpaces> := <space>*
<spaces> := <space>+
<space> := " "
```

`<hueNumber>` indicates the hue (which also indicates the color). It should be a number between 0 and 360.

`<whitenessPercentage>` indicates the whiteness percentage. How ratio of whiteness does it hold? It should be a number between 0 and 100, followed by `%`. For example, `0%`.

`0%` means no saturation, and the color will be always be white.

`100%` means fully saturation.

`<brightnessPercentage>` indicates the brightness percentage. It should be a number between 0 and 100, followed by `%`. For example, `0%`.

+ advanced syntax

```
<hwb> := "hwb("<optionalSpaces><hueNumber><spaces><saturationPercentage><spaces><brightnessPercentage><spaces>"/"<spaces><alphaPercentage><optionalSpaces>")"
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