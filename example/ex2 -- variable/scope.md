# Scope of variable defined in `.css`

To use a variable, it must be declared before with the scope.

The principle of determining the scope of a variable are following:

1. `:root` scope always has higher priority than the other nodes.

2. `html` scope always has higher priority than the other nodes.

3. For all nodes, a node has higher priority than anothor one with same tag of the node, attached with specific either class name, id name, attribute. 

For example, 

- `p` has higher priority than `p.class-name` 

since those affected by `p` in `.css` must be affected by `p.class-name` in `.css`. 

The reason why it is? 

Think about the definition of `p` and `p.class-name` in `.css` file.

- `p` has higher priority than `p[disabled]` 

since those affected by `p` in `.css` must be affected by `p[disabled]` in `.css`. 

- `p.class-name` has higher priority than `p.class-name:hover` 

since those affected by `p.class-name` in `.css` must be affected by `p.class-name:hover` in `.css`. 

> [!TIP]
> Think about hierarchy in `.html` file. 

Recall that the hierarchy of a `.html` file.

```
<!DOCTYPE html5> <!-- REQUIRED -->
<html> <!-- REQUIRED -->
    <head> <!-- OPTIONAL -->
        <style>
        </style>
    </head>
    <header> <!-- OPTIONAL -->
    </header>
    <body> <!-- REQUIRED -->
    </body>
    <footer> <!-- OPTIONAL -->
    </footer>
</html>
```