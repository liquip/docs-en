# Features

A feature is a concept introduced by Liquip. It provides support for modifying items in other ways
than just enchantments.

Features may or may not be tagged.

Untagged features have a value of `null` or `true`.

Tagged features have a value of anything but `null`.

Features are stored in an object called `features` like this one:

```json
{
  "features": {}
}
```

For example, to make your item unbreakable you'd have to write this:

```json
{
  "features": {
    "minecraft:unbreakable": true
  }
}
```

You could also use `null` inplace of `true` as the `minecraft:unbreakable` feature is untagged.

An example of a tagged feature would be this:

```json
{
  "features": {
    "minecraft:dye_leather": "#00FFC0"
  }
}
```

This would make your item - if it was made of leather - colored this specific color.