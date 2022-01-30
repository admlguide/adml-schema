# Entity

An object that participates or is created as part of a business process. 

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | entity                                                       |
| description | An object that participates or is created as part of a business process. |
| version     | 1.0                                                          |

## Attributes 

| Name       | DisplayName | Description                         | DataType | Required? | isNullable |
| ---------- | ----------- | ----------------------------------- | -------- | --------- | ---------- |
| entityID   | Entity ID   | The unique identifier of the Entity | string   | yes       | false      |
| entityName | Entity Name | The name of the Entity              | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Entity was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).     | datetimeoffset | no      | true   |

