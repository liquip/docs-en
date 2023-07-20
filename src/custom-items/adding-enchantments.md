# Adding enchantments

Adding enchantments to items will apply the given enchantments to this item by default.

For example, you could add efficiency 10 to an item like this:

```json
{
  // ...
  "enchantments": [
    {
      "id": "minecraft:efficiency",
      "level": 10
    }
  ]
}
```

Each entry in this list is a new enchantment applied to the item.

Adding unbreaking 4 to it would look like this:

```json
{
  // ...
  "enchantments": [
    {
      "id": "minecraft:efficiency",
      "level": 10
    },
    {
      "id": "minecraft:unbreaking",
      "level": 4
    }
  ]
}
```