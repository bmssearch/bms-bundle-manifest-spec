# Untitled object in bms Schema

```txt
https://bbm.bmssearch.net/schemas/v1/bms.json#/definitions/bms_resource
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                  |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :-------------------------------------------------------------------------- |
| Can be instantiated | No         | Unknown status | No           | Forbidden         | Forbidden             | none                | [bms.schema.json*](../../schemas/v1/bms.schema.json "open original schema") |

# bms_resource Properties

| Property                  | Type      | Required | Nullable       | Defined by                                                                                                                                                   |
| :------------------------ | :-------- | :------- | :------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [url](#url)               | `string`  | Required | cannot be null | [bms](bms-definitions-bms_resource-properties-url.md "https://bbm.bmssearch.net/schemas/v1/bms.json#/definitions/bms_resource/properties/url")               |
| [type](#type)             | `string`  | Required | cannot be null | [bms](bms-definitions-bms_resource-properties-type.md "https://bbm.bmssearch.net/schemas/v1/bms.json#/definitions/bms_resource/properties/type")             |
| [updated_at](#updated_at) | `integer` | Optional | cannot be null | [bms](bms-definitions-bms_resource-properties-updated_at.md "https://bbm.bmssearch.net/schemas/v1/bms.json#/definitions/bms_resource/properties/updated_at") |
| [name](#name)             | `string`  | Optional | cannot be null | [bms](bms-definitions-bms_resource-properties-name.md "https://bbm.bmssearch.net/schemas/v1/bms.json#/definitions/bms_resource/properties/name")             |

## url

url for the resource

`url`

*   is required

*   Type: `string`

## type

core: the main bundle which includes sound sources. patch: files to be overwritten for modification. additional: additional resources such as new patterns.

`type`

*   is required

*   Type: `string`

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

*   Type: `integer`

## name

short description for the resource

`name`

*   is optional

*   Type: `string`
