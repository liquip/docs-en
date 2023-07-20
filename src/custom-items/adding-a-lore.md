# Adding a lore

In Liquip you can add a lore (the lines below the item's name) to your items.

For this you need to create a new list with the name `lore` like so:

```json
{
  // ...
  "lore": []
}
```

You can put strings each representing a new line into this list.

Each individual line - as the item's display name - supports
[MiniMessages](https://docs.advntr.dev/minimessage/format.html).

The default color of each line is purple.

Here's an example of this:

```json
{
  // ...
  "lore": [
    "<blue>This is the first line",
    "This line is purple",
    "<italic>This line is italic"
  ]
}
```