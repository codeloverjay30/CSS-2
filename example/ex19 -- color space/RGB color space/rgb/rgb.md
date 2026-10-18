# rgb()
## syntax 

+ basic syntax

With RE (Regular expression), it can be presented into

```
<rgb> := "rgb("<optionalSpaces><rColorNumber><spaces><gColorNumber><spaces><bColorNumber><spaces><optionalSpaces>")"
```

where

```
<optionalSpaces> := <space>*
<spaces> := <space>+
<space> := " "
```

```
<rColorNumber> := <baseColorNumber>
<gColorNumber> := <baseColorNumber>
<bColorNumber> := <baseColorNumber>


// <baseColorNumber> is a number between 0 to 255 (both inclusive). 
```

+ advance syntax

```
<rgb> := "rgb("<optionalSpaces><rColorNumber><spaces><gColorNumber><spaces><bColorNumber><spaces>"/"<spaces><alphaPercentage><optionalSpaces>")"
```

where 

`<optionalSpaces>` and `<spaces>` are defined in above section.

`<alphaPercentage>` indicates the transparency, it should be a number between 0 and 100 (both inclusive), followed by `%`. (For example, `20%`)

> [!TIP]
> It is same as `rgba()` with following syntax
>
> ```
> <rgba> := "rgba( "<rColorNumber>,<gColorNumber>,<bColorNumber>, <alpha> ")"
> ``` 
> 
> where
> 
> `<alpha>` indicates the transparency, it should be a number between 0 and 1 (both inclusive).
> 
> For more details, see [`rgba.md`](../rgba/rgba.md)

> [!WARNING]
> The advanced syntax of `rgb()`
> 
> ```
> <rgb> := "rgb("<rColorNumber>,<gColorNumber>,<bColorNumber> "/" <alphaPercentage> ")"
> ```
> 
> is only supported on new platform.
>
> As a developer, if you want to develop it for older version of web browser, please consider the other approach.

## color map
See [`color map.png`](../../../color%20map/color%20map.png)