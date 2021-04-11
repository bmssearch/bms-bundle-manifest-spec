# updates Schema

```txt
https://bbm.bmssearch.net/schemas/v1/updates.json
```



| Abstract            | Extensible | Status         | Identifiable | Custom Properties | Additional Properties | Access Restrictions | Defined In                                                                         |
| :------------------ | :--------- | :------------- | :----------- | :---------------- | :-------------------- | :------------------ | :--------------------------------------------------------------------------------- |
| Can be instantiated | Yes        | Unknown status | No           | Forbidden         | Forbidden             | none                | [updates.schema.json](../../schemas/v1/updates.schema.json "open original schema") |

# updates Properties



## version

Bms Bundle Spec version

`version`

*   is required

### version Constraints

**constant**: the value of this property must be equal to:

```json
1
```

## timestamp

current timestamp in millisec

`timestamp`

*   is required

## bmses

bmses which have been updated

`bmses`

*   is optional

# updates Definitions

## Definitions group updates_bms

Reference this group by using

```json
{"$ref":"https://bbm.bmssearch.net/schemas/v1/updates.json#/definitions/updates_bms"}
```



### id

domain scoped identifier

`id`

*   is required

### url

spec url for the bms

`url`

*   is required

### group_id

domain scoped identifier for the group

`group_id`

*   is optional

### updated_at

timestamp in millisec

`updated_at`

*   is optional
