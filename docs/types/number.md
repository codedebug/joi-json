# Type: `number`

The `number` type corresponds to the `Joi.number()` schema.

# String notation
The following example creates some `number` validators:

```js
{
    age: 'number:max=120,positive,integer,required'
    fav_num: 'number:min=1,max=100'
}
```

# Object notation

```js
{
    age: {

        '@type': 'number',
        max: 120,
        positive: true,
        integer: true,
        required: true
    },

    fav_num: {

        '@type': 'number',
        min: 1,
        max: 100
    },
}
```

## Additional properties

Most operations are available including:
- `min`
- `max`
- `required`
- `positive`
- `negative`
- `integer`
- `greater`
- `less`
- `precision`
- `multiple`


For more information on this type, see the [Joi documentation](https://github.com/hapijs/joi/blob/v8/API.md).
