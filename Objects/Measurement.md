# Measurement

A derived measure that supports monitoring and evaluation of performance.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | measurement                                                  |
| description | A derived measure that supports monitoring and evaluation of performance. |
| version     | 1.0                                                          |


## Attributes 

| Name            | DisplayName      | Description                                              | DataType | Required? | isNullable |
| --------------- | ---------------- | -------------------------------------------------------- | -------- | --------- | ---------- |
| measurementID   | Measurement ID   | A unique identifier of the measurement.                  | string   | yes       | false      |
| measurementName | Measurement Name | The name of the measurement.                             | string   | yes       | false      |
| measurementType | Measurement Type | The type of measurement (Outcome, Effectiveness Measure) | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Measurement was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |

## Attribute Reference Data

| Name            | Value                 | Description                                                  |
| --------------- | --------------------- | ------------------------------------------------------------ |
| measurementType | Outcome               | An evaluative measure of a desired business outcome, typically a KPI. |
| measurementType | Effectiveness Measure | A measurement of a business process’ effectiveness, contributing to an outcome |

