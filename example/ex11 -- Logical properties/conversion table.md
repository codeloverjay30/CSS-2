# conversion table from box model to model with logical properties

+ About width

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `width` | `inline-size` |
| `min-width` | `min-inline-size` |
| `max-width` | `max-inline-size` |

+ About height 

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `height` | `block-size` |
| `min-height` | `min-inline-size` |
| `max-height` | `max-inline-size` |

+ About position

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `top` | `inset-block-start` |
| `bottom` | `inset-block-end` |
| `left` | `inset-inline-start` |
| `right` | `inset-inline-end` |

> [!TIP]
> `inset-inline` is abbreviation of `inset-block-start`, `inset-block-end`, `inset-inline-start`, `inset-inline-end`.

+ About margin

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `margin-top` | `margin-block-start` |
| `margin-bottom` | `margin-block-end` |
| `margin-left` | `margin-inline-start` |
| `margin-right` | `margin-inline-end` |

> [!TIP]
> `margin-block` is abbreviation of `margin-block-start`, `margin-block-end`.

> [!TIP]
> `margin-inline` is abbreviation of `margin-inline-start`, `margin-inline-end`.

+ About padding

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `padding-top` | `padding-block-start` |
| `padding-bottom` | `padding-block-end` |
| `padding-left` | `padding-inline-start` |
| `padding-right` | `padding-inline-end` |

> [!TIP]
> `padding-block` is abbreviation of `padding-block-start`, `padding-block-end`.

> [!TIP]
> `padding-inline` is abbreviation of `padding-inline-start`, `padding-inline-end`.

+ About border

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `border-top` | `border-block-start` |
| `border-bottom` | `border-block-end` |
| `border-left` | `border-inline-start` |
| `border-right` | `border-inline-end` |

> [!TIP]
> `border-block` is abbreviation of `border-block-start`, `border-block-end`.

> [!TIP]
> `border-inline` is abbreviation of `border-inline-start`, `border-inline-end`.

+ About floating

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `float: left;` | `float: inline-start;` |
| `float: right;` | `float: inline-end;` |
 
+ About text-align

| Box model | model with logical properties |
| ---------- | ---------------------------- |
| `text-align: left;` | `text-align: start;` |
|`text-align: right;` | `text-align: end;` |

+ About flex
In fields about flex, there are same in box model and model with logical properties 

since fields about flex can do anything what model with logical properties does. 

+ About grid
In fields about grid, there are same in box model and model with logical properties 

since fields about grid can do anything what model with logical properties does. 
