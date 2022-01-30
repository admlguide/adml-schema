# Imperative-Measurement Bridge

Associates an imperative with many measurements.

## Properties

| Property    | Value                                            |
| ----------- | ------------------------------------------------ |
| name        | imperative-measurement                           |
| description | Associates an imperative with many measurements. |
| version     | 1.0                                              |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| measurementID | Measurement ID | The unique identifier of the Measurement | string   | yes       | false      |
| imperativeID | Imperative ID | The unique identifier of the Imperative | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the item was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).  | datetimeoffset | no      | true   |
