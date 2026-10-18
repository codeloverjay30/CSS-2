# hsb()
## syntax 

+ basic syntax

With RE (Regular expression), it can be presented into

```
<hsb> := "hsb("<optionalSpaces><hueNumber><spaces><saturationPercentage><spaces><brightnessPercentage><optionalSpaces>")"
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

`<brightnessPercentage>` indicates the brightness percentage. It should be a number between 0 and 100, followed by `%`. For example, `0%`.

+ advanced syntax

```
<hsb> := "hsb("<optionalSpaces><hueNumber><spaces><saturationPercentage><spaces><brightnessPercentage><spaces>"/"<spaces><alphaPercentage><optionalSpaces>")"
```

where

`<optionalSpaces>` and `<spaces>` are defined in above section.

`<alphaPercentage>` indicates the transparency, it should be a number between 0 and 100 (both inclusive), followed by `%`. (For example, `20%`)

> [!TIP]
> It is same as `hsba()` with following syntax
>
> ```
> <hsba> := "hsba("<optionalSpaces><hueNumber><comma><saturationPercentage><comma><brightnessPercentage><comma><alpha><optionalSpaces>")"
> ``` 
> 
> where
> 
> `<alpha>` indicates the transparency, it should be a number between 0 and 1 (both inclusive).
> 
> For more details, see [`hsba.md`](../hsba/hsba.md)

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