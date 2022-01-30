# Learning

The documented findings from a learning review session.

## Properties

| Property    | Value                                                   |
| ----------- | ------------------------------------------------------- |
| name        | learning                                                |
| description | The documented findings from a learning review session. |
| version     | 1.0                                                     |

## Attributes 

| Name                  | DisplayName             | Description                                                  | DataType | Required? | isNullable |
| --------------------- | ----------------------- | ------------------------------------------------------------ | -------- | --------- | ---------- |
| learningID            | Learning ID             | The unique identifier of the learning review                 | string   | yes       | false      |
| dataProductID         | Data Product ID         | The related Data Product which is the topic of the learning review | string   | yes       | false      |
| precedent             | Precedent               | Textual summary of where the undertakings of the data product have been attempted before. | string   | no        | true       |
| history               | History                 | Textual summary of what previous undertakings resulted in.   | string   | no        | true       |
| differenceToPrecedent | Difference to Precedent | Textual summary of how the Data Product varies in circumstances and outcomes to previous undertakings. | string   | no        | true       |
| conclusion            | Conclusion              | Textual summary of how the Data Product should be refined or used in the future. | string   | yes       | false      |
| period                | Period                  | The period of time for which the review covers.              | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Learning findings were updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |



