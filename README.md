# elixir-cheatsheet

## Basic stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`len(x)` | `x |> length`|
|`min(1, 2)` | `[1, 2] |> Enum.min`|

## String stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`"a,b,c".split(',')` | `"a,b,c" |> String.split(",")`|
|`["a", "b"].join(",")` | `["a", "b"] |> Enum.join(",")`|
| String replace | `"abc" |> String.replace("b", "B")` |
| String slice | `"abc" |> String.slice(0..1)`|

## Regex

`String.replace(~r/\<.*\>/U, "<i>hi</i>"`

## Array access

| Python 	| Elixir 	|
|-------- |--------	|
|`arr[0]` | `arr |> Enum.at(0)`|
|`arr[1:]` | `arr |> Enum.slice(1..-1)`|
|`arr[a:b]` | `arr |> Enum.slice(a..b-1)` |
|`arr[::-1]` | `arr |> Enum.reverse` |

## Dictionary

| Python 	| Elixir 	|
|-------- |--------	|
|`dic['w']` | `dic |> Map.fetch!("w")`|
|`dic.values()` | `dic |> Map.values`|

## Functional stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`[f(x) for x in xs]` | `xs |> Enum.map(fn x -> f x end)`|
|`[x for x in xs if p(x)` | `xs |> Enum.filter(fn x -> p x end)`|

## Hash stuff

```
    hash = :crypto.hash(:sha, contents)
    |> Base.encode16
    |> String.downcase
```
