# Data Readiness

Validation of whether data exists in a form that will support the analytics objectives.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | dataReadiness                                                |
| description | Validation of whether data exists in a form that will support the analytics objectives. |
| version     | 1.0                                                          |

## Attributes 

| Name                       | DisplayName                 | Description                                                  | DataType | Required? | isNullable |
| -------------------------- | --------------------------- | ------------------------------------------------------------ | -------- | --------- | ---------- |
| dataReadinessID            | Data Readiness ID           | The unique identifier of the data readiness set of observations | string   | yes       | false      |
| dataProductID              | Data Product ID             | The associated Data Product for which data readiness is being assessed | string   | yes       | false      |
| availabilityRating         | Availability Rating         | A rating of the ease at which data can be acquired in a timely and repeatable manner | string   | yes       | false      |
| availabilityDescription    | Availability Description    | Explanatory text relating the Availability Rating            | string   | no        | true       |
| clarityRating              | Clarity Rating              | A rating of how well understood the meaning of data is       | string   | yes       | false      |
| clarityDescription         | Clarity Description         | Explanatory text relating the Clarity Rating                 | string   | no        | true       |
| coverageRating             | Coverage Rating             | A rating of how well data is captured as part of a business process | string   | yes       | false      |
| coverageDescription        | Coverage Description        | Explanatory text relating the Coverage Rating                | string   | no        | true       |
| consistencyRating          | Consistency Rating          | A rating of the level of variation in data captured          | string   | yes       | false      |
| consistencyDescription     | Consistency Description     | Explanatory text relating the Consistency Rating             | string   | no        | true       |
| authorityRating            | Authority Rating            | A rating of whether the best source of data has been made available or has been agreed | string   | yes       | false      |
| authorityDescription       | Authority Description       | Explanatory text relating the Authority Rating               | string   | no        | true       |
| cross-RelatableRating      | Cross-Relatable Rating      | A rating of how reliably data can be related between entities and processes. | string   | yes       | false      |
| cross-RelatableDescription | Cross-Relatable Description | Explanatory text relating the Cross-Relatable Rating         | string   | no        | true       |
| modifiedDateTime| Modified DateTime | The most recent time that the specific set of Data Readiness observations were updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |

## Attribute Reference Data

| Name            | Value                 | Description                                                  |
| --------------- | --------------------- | ------------------------------------------------------------ |
| [Category]Rating | 1 | Inadequate |
| [Category]Rating | 2 | Limited |
| [Category]Rating | 3 | Fair |
| [Category]Rating | 4 | Good |
| [Category]Rating | 5 | Exceptional |



