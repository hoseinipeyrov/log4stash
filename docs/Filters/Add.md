Filters - Add
=====================

Adding new tag to the log event.

Configuration example:

```xml
<ElasticFilters>
    <Add>
        <Key>TagName</Key>
        <Value>TagValue</Value>
        
        <!-- optional -->
        <Overwrite>True</Overwrite>
    </Add>
</ElasticFilters>
```
### Properties:

#### Key
The name of the tag.
You can use here [smart formatting][smart-formatting].

#### Value
The value.
You can use here [smart formatting][smart-formatting].

#### Overwrite
Whether to overite or append if this tag already exists.

For example if you have tag with the name `Address` and value `first` and you using the Add filter to add `Address` with value of `second`.<br />
If the `Overwrite` is true - The original address will be replaced with `second`.<br />
If the `Overwrite` is false - The tag `Address` will be replace by array with the values `['first', 'second']`.
