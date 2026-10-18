# hsb()
## syntax 

+ basic syntax

With RE (Regular expression), it can be presented into

```
<hsl> := "hsl("<optionalSpaces><hueNumber><spaces><saturationPercentage><spaces><lightnessPercentage><optionalSpaces>")"
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

+ advanced syntax

```
<hsl> := "hsl("<optionalSpaces><hueNumber><spaces><saturationPercentage><spaces><lightnessPercentage><spaces>"/"<spaces><alphaPercentage><optionalSpaces>")"
```

where

`<optionalSpaces>` and `<spaces>` are defined in above section.

`<alphaPercentage>` indicates the transparency, it should be a number between 0 and 100 (both inclusive), followed by `%`. (For example, `20%`)

> [!TIP]
> It is same as `hsla()` with following syntax
>
> ```
> <hsla> := "hsla("<optionalSpaces><hueNumber><comma><saturationPercentage><comma><lightnessPercentage><comma><alpha><optionalSpaces>")"
> ``` 
> 
> where
> 
> `<alpha>` indicates the transparency, it should be a number between 0 and 1 (both inclusive).
> 
> For more details, see [`hsla.md`](../hsla/hsla.md)

> [!WARNING]
> The advanced syntax of `hsb()`
> 
> ```
> <hsb> := "hsb("<rColorNumber>,<gColorNumber>,<bColorNumber> "/" <alphaPercentage> ")"
> ```
> 
> is only supported on new platform.
>
> As a developer, if you want to develop it for older version of web browser, please consider the other approach.