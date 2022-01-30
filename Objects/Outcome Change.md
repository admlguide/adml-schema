# Outcome Change

The desired change in an outcome that will result from the issue being successfully addressed.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | outcomeChange                                                |
| description | The desired change in an outcome that will result from the issue being successfully addressed. |
| version     | 1.0                                                          |

## Attributes 

| Name                     | DisplayName                 | Description                                         | DataType | Required? | isNullable |
| ------------------------ | --------------------------- | --------------------------------------------------- | -------- | --------- | ---------- |
| outcomeChangeID          | Outcome Change ID           | The unique identifier of the outcome change.        | string   | yes       | false      |
| outcomeChangeName        | Outcome Change Name         | The name of the outcome change.                     | string   | yes       | false      |
| outcomeChangeTargetValue | Outcome Change Target Value | The target amount of change to measure improvement. | string   | yes       | false      |
| issueID | Issue ID | The unique identifier of the related issue | string | yes | false |
| modifiedDateTime| Modified DateTime | The most recent time that the Outcome Change was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |

