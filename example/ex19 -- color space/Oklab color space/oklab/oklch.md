# oklch
## syntax

+ basic syntax

With RE (Regular expression), it can be presented into

```
<oklch> := "oklch("<optionalSpaces><lightnessPercentage><spaces><chromaPercentage><spaces><hueNumber><optionalSpaces>")"
```

where

```
<optionalSpaces> := <space>*
<spaces> := <space>+
<space> := " "
```

`<lightnessPercentage>` indicates the lightness percentage. It should be a number between 0 and 100, followed by `%`. For example, `0%`.

`<chromaPercentage>` indicates the chroma percentage. It should be a number between 0 and 100, followed by `%`. For example, `0%`.

`<hueNumber>` indicates the hue (which also indicates the color). It should be a number between 0 and 360.

+ advanced syntax

```
<oklch> := "oklch("<optionalSpaces><lightnessPercentage><spaces><chromaPercentage><spaces><hueNumber><spaces>"/"<alphaPercentage><optionalSpaces>")"
```

where

`<optionalSpaces>` and `<spaces>` are defined in above section.

`<alphaPercentage>` indicates the transparency, it should be a number between 0 and 100 (both inclusive), followed by `%`. (For example, `20%`)

> [!WARNING]
> The advanced syntax of `oklch()`
> 
> ```
> <oklch> := "oklch("<optionalSpaces><lightnessPercentage><spaces><chromaPercentage><spaces><hueNumber><spaces>"/"<alphaPercentage><optionalSpaces>")"
> ```
> 
> is only supported on new platform.
>
> As a developer, if you want to develop it for older version of web browser, please consider the other approach.

> [!WARNING]
> There are no `oklcha()` function in native CSS.