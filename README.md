# elixir-cheatsheet

## String stuff

| Python 	| Elixir 	|
|-------- |--------	|
|`"a,b,c".split(',')` | `"a,b,c" \|\> String.split(",")`|
|`["a", "b"].join(",")` | `["a", "b"] \|\> Enum.join(",")`|


## Array slicing stuff

| Python 	| Elixir 	|
|-------- |--------	|
|arr[0] | arr \|\> Enum.at(0)|
|arr[0:] | arr \|\> Enum.slice(1..-1)
