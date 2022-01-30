# Intervention

The things we can change to bring about an outcome change.

## Properties

| Property    | Value                                                      |
| ----------- | ---------------------------------------------------------- |
| name        | intervention                                               |
| description | The things we can change to bring about an outcome change. |
| version     | 1.0                                                        |

## Attributes 

| Name             | DisplayName       | Description                                | DataType | Required? | isNullable |
| ---------------- | ----------------- | ------------------------------------------ | -------- | --------- | ---------- |
| interventionID   | Intervention ID   | The unique identifier of the Intervention. | string   | yes       | false      |
| interventionName | Intervention Name | The name of the Intervention.              | string   | yes       | false      |
| driverID         | Driver ID         | The reference to the related Driver.       | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Intervention was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |

