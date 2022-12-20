# Minimal item config

The minimal config that you put inside your item files looks like this:

```json
{
  "key": "test:test_item",
  "material": "minecraft:paper",
  "displayName": "<blue>Test Item"
}
```

In the next chapters you will learn about more features of the item configuration but for now this
is all you will need.

The `key` field is the key your item will be identified with. It consists of a first part, the
namespace, and a second part the key. The namespace should be the name of the group of items you
want to create or for plugin developers the name of their plugin. The both parts should be all
lowercase and may separate words with underscores. The second part may contain slashes to further
group items.[^resource-location]

The `material` field is a simple minecraft item identifier used in command. You can find these on
the [unofficial Minecraft Wiki](https://minecraft.fandom.com/wiki/Minecraft_Wiki)'s page of the
item. For paper for example you can find the key [here](https://minecraft.fandom.com/wiki/Paper#ID).
The namespace will always be `minecraft`.

The `displayName` field is a [MiniMessage](https://docs.adventure.kyori.net/minimessage/format.html)
component. This allows you to format the name of your item with "modern" features like RGB colors.

This will add a new item with the identifier `test:test_item` made out of paper to Liquip. If you
give it to yourself with `/liquip give test:test_item` it will have the name `Test Item` colored in
blue.

[^resource-location] For further information read
[this](https://minecraft.fandom.com/wiki/Resource_location).