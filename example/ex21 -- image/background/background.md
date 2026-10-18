# background
## shorthand
> [!NOTE]
> `background` field is a shorthand of `background-color` `background-image` `background-attachment` `background-repeat` `background-position` / `background-size`.

## syntax
```
<background> := <background-color><spaces><background-image><spaces><background-attachment><spaces><background-repeat><spaces><background-position>"/"<spaces><background-size>
```

where 

```
<spaces> := <space>+
<space> := " "
```

and 

`<background-color>` is `background-color` field.

`<background-image>` is `background-image` field.

`<background-attachment>` is `background-attachment` field.

`<background-repeat>` is `background-repeat` field.

`<background-position>` is `background-position` field.

`<background-size>` is `background-size` field.

## example
```
	background: 
				#eee  						/* background-color */
				url("images/avatar.jpg")	 /* background-image */
				scroll						 /* background-attachment */
				repeat						 /* background-repeat */
				center						 /* background-position */
				/ 
				cover 						 /* background-size */
```

For more example, see `background ex1.css` and `background ex2.css` examples.