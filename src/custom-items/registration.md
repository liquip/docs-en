# Registration

The files for the items must be placed in a specific location and must be registered in the main
config.

## File structure

The file structure in the directory `plugins/liquip` should currently look something like this:

```
.
└── config.json
```

To now add items you want to create a new directory to store your item files.

Best is to name it something like `items`.

In this directory you can put your item files directly or make subdirectories for each namespace.

Here you can see an example:

```
.
├── config.json
└── items
    └── mynewitems
        ├── bedrock_pickaxe.json
        └── bedrock_sword.json
```

For each new item you add, you will create a new file there.

## Registration

To register your items you have to add a new entry to the `items` list in the `config.json` file in
the directory `plugins/liquip` with the path to the item file.

For the example shown above it would look something like this:

```json
{
  "items": [
    "items/mynewitems/bedrock_pickaxe.json",
    "items/mynewitems/bedrock_sword.json"
  ]
}
```
