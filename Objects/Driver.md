# Driver

The variables that are related to the outcome change.

## Properties

| Property    | Value                                                |
| ----------- | ---------------------------------------------------- |
| name        | driver                                               |
| description | The variables that are related to the outcome change |
| version     | 1.0                                                  |

## Attributes 

| Name                           | DisplayName                       | Description                                                  | DataType | Required? | isNullable |
| ------------------------------ | --------------------------------- | ------------------------------------------------------------ | -------- | --------- | ---------- |
| driverID                       | Driver ID                         | The unique identifier of the driver.                         | string   | yes       | false      |
| driverName                     | Driver Name                       | The name of the driver.                                      | string   | yes       | false      |
| outcomeChangeID                | Outcome Change ID                 | The reference to the primary related outcome.                | string   | yes       | false      |
| outcomeDriverContributionName  | Outcome Driver Contribution Name  | The name of the measure of contribution towards the outcome. | string   | no        | true       |
| outcomeDriverContributionValue | Outcome Driver Contribution Value | The quantified measurement of contribution towards the outcome. | string   | no        | true       |
| modifiedDateTime| Modified DateTime | The most recent time that the Driver was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |

