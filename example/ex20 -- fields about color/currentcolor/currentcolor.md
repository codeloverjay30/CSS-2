# `currentcolor` keyword
The `currentcolor` records the current color. 

> [!NOTE]
> **DON'T** set the current color through `currentcolor` such as DON'T do `currentcolor: blue;`
> 
> To set the current color, simply set value in `color` field such as `color:blue`. It has mentioned before.

> [!NOTE]
> For correctness, you must use `currentcolor` after assignment of `color` field (if there exists) since the CSS parser parse the code from top to bottom.
> 
> **NEVER** do, for example
> 
> ```
> h1 {
>   color: blue; /* Blue text color */
>   border: 10px solid currentcolor; /* Blue border color */  
> }
> ```
> 
> Otherwise, you may get the old color when accessing value with `currentcolor` (here, it may NOT be blue when accessing value with `currentcolor`).