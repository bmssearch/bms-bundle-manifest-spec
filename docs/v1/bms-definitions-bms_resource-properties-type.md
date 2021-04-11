# Untitled string in bms Schema

```txt
https://bbm.bmssearch.net/schemas/v1/bms.json#/definitions/bms_resource/properties/type
```

core: the main bundle which includes sound sources. patch: files to be overwritten for modification. additional: additional resources such as new patterns.

| Abstract            | Extensible | Status         | Identifiable            | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                  |
| :------------------ | :--------- | :------------- | :---------------------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | Unknown identifiability | Forbidden         | Allowed               | none                | [bms.schema.json*](../../schemas/v1/bms.schema.json "open original schema") |

## type Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | :---------- |
| `"core"`       |             |
| `"patch"`      |             |
| `"additional"` |             |
