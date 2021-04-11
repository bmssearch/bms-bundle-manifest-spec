# resource Schema

```txt
https://bbm.bmssearch.net/schemas/v1/bms.schema.json#/definitions/bms_resource
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                  |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [bms.schema.json*](../../schemas/v1/bms.schema.json "open original schema") |

# bms_resource Properties



## url

url for the resource

`url`

*   is required

## type

core: the main bundle which includes sound sources. patch: files to be overwritten for modification. additional: additional resources such as new patterns.

`type`

*   is required

### type Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | :---------- |
| `"core"`       |             |
| `"patch"`      |             |
| `"additional"` |             |

## updated_at

timestamp in millisec

`updated_at`

*   is optional

## name

short description for the resource

`name`

*   is optional
