# [`@media`](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)
## syntax

With [`RE (regular expression)`](https://learn.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference), it can be expressed into

```
<mediaAnnotaion> := @media <conditions> { <statements> }
```

Where

```
<statements> := <statement>*

<statement> := <fieldValuePair> ";"

<fieldValuePair> := <field> ":" <value>
```

```
<conditions> := <condition> (<binaryLogicalOperator> <condition>)*

<condition> := <negativeCondition> | <postiveCondition>

<negativeCondition> := <negationOperator> <postiveCondition>

<negationOperator> := "not" 

<postiveCondition> :=  <postiveCondition> | "("<postiveCondition>")"
<postiveCondition> := <booleanExpression>

// <booleanExpression> is a boolean expression (i.e. an expression that returns boolean (true or false)).

<binaryLogicalOperator> := "and" | "," 
```

