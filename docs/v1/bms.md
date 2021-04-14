# bms Schema

```txt
https://bbm.bmssearch.net/schemas/v1/bms.schema.json
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                 |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :------------------------------------------------------------------------- |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Forbidden             | none                | [bms.schema.json](../../schemas/v1/bms.schema.json "open original schema") |

# bms Properties



## version

Bms Bundle Manifest Spec version

`version`

*   is required

### version Constraints

**constant**: the value of this property must be equal to:

```json
1
```

## id

domain scoped identifier

`id`

*   is required

## title

title

`title`

*   is required

## aliases

bms manifests which can be treated as the same bms

`aliases`

*   is optional

## website_url

website

`website_url`

*   is optional

## group_urls

spec url for the group to which this bms belongs

`group_urls`

*   is optional

## updates_url

spec url to check for updates on this bms

`updates_url`

*   is optional

## resources

resources for this bms

`resources`

*   is required

# bms Definitions

## Definitions group bms_alias

Reference this group by using

```json
{"$ref":"https://bbm.bmssearch.net/schemas/v1/bms.schema.json#/definitions/bms_alias"}
```



### domain

domain to which the alias manifest belongs

`domain`

*   is required

### id

domain scoped id of the alias manifest

`id`

*   is required

## Definitions group bms_resource

Reference this group by using

```json
{"$ref":"https://bbm.bmssearch.net/schemas/v1/bms.schema.json#/definitions/bms_resource"}
```



### url

url for the resource

`url`

*   is required

### type

core: the main bundle which includes sound sources. patch: files to be overwritten for modification. additional: additional resources such as new patterns.

`type`

*   is required

#### type Constraints

**enum**: the value of this property must be equal to one of the following values:

| Value          | Explanation |
| :------------- | :---------- |
| `"core"`       |             |
| `"patch"`      |             |
| `"additional"` |             |

### updated_at

timestamp in millisec

`updated_at`

*   is optional

### name

short description for the resource

`name`

*   is optional
