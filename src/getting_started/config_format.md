# The Config Format

Many plugins use the [YAML configuration-language](https://en.wikipedia.org/wiki/YAML). We instead use a different
config-format. We think it is less error-prone as it does not rely on indentation. It is called HOCON and we recommend
the `.conf` file-extension. You can read more about
it [here](https://github.com/lightbend/config/blob/4458ea947a7a2a668bb811a122455f1f05975172/HOCON.md), but we will also
explain the basics in this short guide.

## Data types

In HOCON there are the following data types:

* Object
* List
* Integer
* Floating-point number
* String/Text
* Boolean (true/false)

## Representation

The config-file itself is an object. It contains key-value pairs. To assign a value to a key you write the key followed
by an equals-sign (`=`) or a colon (`:`) followed by the value. This will look like this:

```hocon
some_value: 42
```

or

```hocon
some_other_value: 13
```

### Simple types

Integers are just written-out (e.g. `123`).

Floats are written with a dot as separator (e.g. `4.5`).

Strings are written in double-quotes (e.g. `"Hello, world!"`).

Booleans are written as true or false (e.g. `true`).

### Objects

Objects are written as key-value pairs surrounded by curly-braces (`{}`) separated by commas or newlines.

Assigning an object to a key may look like this:

```hocon
some_object: {some_string = "Hey", some_number = 456}
```

or this:

```hocon
some_other_object: {
  some_other_string: "Hey"
  some_other_number: 456
}
```

### Lists

Lists are written as values surrounded by square-brackets (`[]`) separated by commas or newlines.

This may look like this:

```hocon
some_list: [1, 2.0, "three"]
```

or like this:

```hocon
some_other_list: [
  1
  2.0
  "three"
]
```
