# Imperative

An overarching theme for a set of related improvement objectives. 

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | imperative                                                   |
| description | An overarching theme for a set of related improvement objectives.  |
| version     | 1.0                                                          |

## Attributes 

| Name           | DisplayName     | Description                             | DataType | Required? | isNullable |
| -------------- | --------------- | --------------------------------------- | -------- | --------- | ---------- |
| imperativeID   | Imperative ID   | A unique identifier for each imperative | string   | yes       | false      |
| imperativeName | Imperative Name | The name of the imperative      | string   | yes       | false      |
| processAreaID  | Process Area ID | The related Process Area                | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Imperative was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |

