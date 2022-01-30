# Activity-Entity Bridge

Associates activities and entities.

## Properties

| Property    | Value                               |
| ----------- | ----------------------------------- |
| name        | activity-entity                     |
| description | Associates activities and entities. |
| version     | 1.0                                 |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| activityID   | Activity ID   | The unique identifier of the Activity | string   | yes       | false      |
| entityID | Entity ID | The unique identifier of the Entity | string   | yes       | false      |
| modifiedDateTime | Modified DateTime | The most recent time that the item was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601). | datetimeoffset | no        | true       |
