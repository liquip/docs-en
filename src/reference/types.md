# Types

| Name       | Description                                    |   Example   |
|------------|------------------------------------------------|:-----------:|
| Integer    | Number without decimal point                   |    `42`     |
| Float      | Number with optional decimal point             |    `1.5`    |
| String     | Text surrounded by double quotes               |  `"Hello"`  |
| Hex string | Hexadecimal number with hashtag in front of it | `"#0ABCDE"` |

## Attribute modifier

An attribute modifier may be an object or a list of objects.

Each object has the following fields:

* attribute: `Attribute`
* name: `String`
* amount: `Float`
* operation: `"+"`/`"*"`

If `operation` is `"+"`, `amount` will be added to the `attribute`.

If `operation` is `"*"`, `attribute`'s value will be multiplied by `amount` + 1.
This means it will show up as e.g. `+50%`.

### Example

```json
{
    "attribute": "generic_attack_damage",
    "name": "myAttackDamageModifier",
    "amount": 0.5,
    "operation": "*"
}
```

## Attribute

An attribute is one of the following strings representing an attribute of an entity:

| String                         | Description                                 |
|--------------------------------|---------------------------------------------|
| `generic_armor`                | Armor                                       |
| `generic_armor_toughness`      | Armor durability                            |
| `generic_attack_damage`        | Attack damage                               |
| `generic_attack_knockback`     | Attack knock-back                           |
| `generic_attack_speed`         | Attack speed                                |
| `generic_flying_speed`         | Flying speed                                |
| `generic_follow_range`         | Range at which an entity will follow others |
| `generic_knockback_resistance` | Resistance to knock-back                    |
| `generic_luck`                 | Luck bonus                                  |
| `generic_max_health`           | Maximum health                              |
| `generic_movement_speed`       | Movement speed                              |
| `horse_jump_strength`          | Horse's jumping strength                    |
| `zombie_spawn_reinforcements`  | Chance of a zombie spawning reinforcements  |
