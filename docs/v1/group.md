# group Schema

```txt
https://bbm.bmssearch.net/schemas/v1/group.schema.json
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                     |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :----------------------------------------------------------------------------- |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Forbidden             | none                | [group.schema.json](../../schemas/v1/group.schema.json "open original schema") |

# group Properties



## version

Bms Bundle Spec version

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

## name

name

`name`

*   is required

## aliases

group manifests which can be treated as the same group

`aliases`

*   is optional

## website_url

website

`website_url`

*   is optional

## updates_url

spec url to check for updates on bmses in this group

`updates_url`

*   is optional

## bmses

bmses in this group

`bmses`

*   is optional

# group Definitions

## Definitions group group_alias

Reference this group by using

```json
{"$ref":"https://bbm.bmssearch.net/schemas/v1/group.schema.json#/definitions/group_alias"}
```



### domain

domain to which the alias manifest belongs

`domain`

*   is required

### id

domain scoped id of the alias manifest

`id`

*   is required

## Definitions group group_bms

Reference this group by using

```json
{"$ref":"https://bbm.bmssearch.net/schemas/v1/group.schema.json#/definitions/group_bms"}
```



### id

domain scoped identifier

`id`

*   is required

### url

spec url for the bms

`url`

*   is required
