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

## Regex

`String.replace(~r/\<.*\>/U, "<i>hi</i>"`

## Array/Dictionary access

| Python 	| Elixir 	|
|-------- |--------	|
|`arr[0]` | `arr |> Enum.at(0)`|
|`dic['w']` | `dic |> Map.fetch!("w")`|
|`arr[1:]` | `arr |> Enum.slice(1..-1)`|
|`arr[a:b]` | `arr |> Enum.slice(a..b-1)` |

## Functional stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`[f(x) for x in xs]` | `xs |> Enum.map(fn x -> f x end)`|
|`[x for x in xs if p(x)` | `xs |> Enum.filter(fn x -> p x end)`|
