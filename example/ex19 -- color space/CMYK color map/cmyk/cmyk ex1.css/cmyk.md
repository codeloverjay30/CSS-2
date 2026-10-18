# cmyk()
## syntax

With RE (Regular expression), it can be presented into

```
<cmyk> := "cmyk("<optionalSpaces><cColorPercentage><comma><mColorPercentage><comma><yColorPercentage><comma><kColorPercentage><optionalSpaces>")"
```

where 

```
<comma> := ","
<optionalSpaces> := <space>*
<space> := " "
```

```
<cColorPercentage> := <colorPercentage> 
<mColorPercentage> := <colorPercentage> 
<yColorPercentage> := <colorPercentage> 
<kColorPercentage> := <colorPercentage> 
```

`<colorPercentage>` must be a number between 0 to 100, followed by a `%`. For example, `100%`.


## color map
See [`color map.png`](../../../color%20map/color%20map.png)