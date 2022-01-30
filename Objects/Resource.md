# Resource

A person or technology which records data.

## Properties

| Property    | Value                                      |
| ----------- | ------------------------------------------ |
| name        | resource                                   |
| description | A person or technology which records data. |
| version     | 1.0                                        |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| resourceID   | Resource ID   | The unique identifier of the Resource | string   | yes       | false      |
| resourceName | Resource Name | The name of the Resource              | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Resource was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |

