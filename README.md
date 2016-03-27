# elixir-cheatsheet

## Basic stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`len(x)` | `x |> length`|

## String stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`"a,b,c".split(',')` | `"a,b,c" |> String.split(",")`|
|`["a", "b"].join(",")` | `["a", "b"] |> Enum.join(",")`|


## Array/Dictionary access

| Python 	| Elixir 	|
|-------- |--------	|
|`arr[0]` | `arr |> Enum.at(0)`|
|`dic['w']` | `dic |> Map.fetch!("w")`|
|`arr[0:]` | `arr |> Enum.slice(1..-1)`|

## Functional stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`[f(x) for x in xs]` | `xs |> Enum.map(fn x -> f x end)`|
|`[x for x in xs if p(x)` | `xs |> Enum.filter(fn x -> p x end)`|
