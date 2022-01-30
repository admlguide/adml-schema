# Activity-Measurement Bridge

Associates a measurement with many activities.

## Properties

| Property    | Value                                         |
| ----------- | --------------------------------------------- |
| name        | activity-measurement                          |
| description | Associates a measurement with many activities |
| version     | 1.0                                           |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| activityID   | Activity ID   | The unique identifier of the Activity | string   | yes       | false      |
| measurementID | Measurement ID | The unique identifier of the Measurement | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the item was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).  | datetimeoffset | no      | true   |
