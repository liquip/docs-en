# The Config Format

Liquip uses a modified version of [JSON](https://en.wikipedia.org/wiki/JSON) for all of its config
files.

If you don't know JSON yet, you easily learn it with the Wikipedia article.

[This](https://en.wikipedia.org/wiki/JSON#Data_types) position is especially important.

## Differences

Liquip allows the following things:
* unquoted field names
* comments
* single quotes

So you might do something like this:

```js
{
    // some comment
    name: 'value',
    'otherName': "otherValue"
}
```
