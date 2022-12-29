# Attribute modifiers

Minecraft has a concept called attribute modifiers. It allows you to modify things like movement 
speed of players.

In the context of item creation they allow you to modify these things for the player holding or 
wearing your item.

An item may have none to several attribute modifiers.

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

> **This page is not done yet.**