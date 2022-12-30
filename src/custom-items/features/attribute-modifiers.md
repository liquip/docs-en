# Attribute modifiers

Minecraft has a concept called attribute modifiers. It allows you to modify things like movement
speed of players.

In the context of item creation they allow you to modify these things for the player holding or
wearing your item.

An item may have none to several attribute modifiers.

## Single attribute modifier

A single attribute modifier looks like this:

```json
{
  "features": {
    "minecraft:attribute_modifier": {
      "name": "myAttributeModifier",
      "attribute": "generic_movement_speed",
      "amount": 0.25,
      "operation": "*",
      "slot": "feet"
    }
  }
}
```

This will give every player wearing the item on their feet a 25% speed boost.

The `name` field is just a string to indicate from where the attribute modifier came.

The field called `attribute` specifies what attribute should be changed. Possible values can be
found [here](https://liquip.github.io/docs-en/reference/types.html#attribute).

The amount the attribute should be changed by is indicated by `amount`.

The amount can either be just added by setting `operation` to `+` or added in percent of the
original by setting `operation` to `*`. Last will, for example, for a base damage amount of 10 and
an attribute amount of 0.4 add 40% (or 4 damage) to the total damage. After appliance the damage
will be 14.

The `slot` represents what slot a player need to wear the item in to get the attribute modifiers
applied to themselves. Possible values are can be found
[here](https://liquip.github.io/docs-en/reference/types.html#slot).

## Several attribute modifiers

To add more attribute modifiers to one item you put them in a list like so:

```json
{
  "features": {
    "minecraft:attribute_modifier": [
      {
        "name": "myAttributeModifier",
        "attribute": "generic_movement_speed",
        "amount": 0.25,
        "operation": "*",
        "slot": "feet"
      },
      {
        "name": "myOtherAttributeModifier",
        "attribute": "generic_attack_damage",
        "amount": 5,
        "operation": "+",
        "slot": "feet"
      }
    ]
  }
}
```