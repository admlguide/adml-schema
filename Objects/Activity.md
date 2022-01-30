# Activity

An event or series of events that occur as part of a business process.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | activity                                                     |
| description | An event or series of events that occur as part of a business process. |
| version     | 1.0                                                          |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| activityID   | Activity ID   | The unique identifier of the Activity | string   | yes       | false      |
| activityName | Activity Name | The name of the Activity              | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Activity was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |
