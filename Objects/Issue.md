# Issue

An existing or potential problem affective process imperatives and the ability to achieve goals.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | issue                                                        |
| description | An existing or potential problem affective process imperatives and the ability to achieve goals. |
| version     | 1.0                                                          |

## Attributes 

| Name      | DisplayName | Description                       | DataType | Required? | isNullable |
| --------- | ----------- | --------------------------------- | -------- | --------- | ---------- |
| issueID   | Issue ID    | The unique identifier of an issue | string   | yes       | false      |
| issueName | Issue Name  | The name of the issue             | string   | yes       | false      |
| hypothesisID | Hypothesis ID | The unique identifier of the related Hypothesis | string | yes | false |
| modifiedDateTime| Modified DateTime | The most recent time that the Issue was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |



