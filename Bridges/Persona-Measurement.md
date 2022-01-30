# Persona-Measurement Bridge

Associates a persona with many measurements.

## Properties

| Property    | Value                                        |
| ----------- | -------------------------------------------- |
| name        | persona-measurement                          |
| description | Associates a persona with many measurements. |
| version     | 1.0                                          |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| personaID | Persona ID | The unique identifier of the Persona | string   | yes       | false      |
| measurementID | Measurement ID | The unique identifier of the Measurement | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Activity was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no     | true |
