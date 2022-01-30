# Data Product Benefit

Tracking of benefits of a data product over time.

## Properties

| Property    | Value                                             |
| ----------- | ------------------------------------------------- |
| name        | dataProductBenefit                                |
| description | Tracking of benefits of a data product over time. |
| version     | 1.0                                               |

## Attributes 

| Name          | DisplayName     | Description                                              | DataType | Required? | isNullable |
| ------------- | --------------- | -------------------------------------------------------- | -------- | --------- | ---------- |
| dataProductBenefitID | Data Product Benefit ID | A unique identifier for the Data Product Benefit | string | yes | false |
| dataProductID | Data Product ID | A reference to which Data Product the benefits relate | string   | yes       | false      |
| benefitName   | Benefit Name    | The name of the benefit                                  | string   | yes       | false      |
| benefitAmount | Benefit Amount  | The quantified amount of benefit                         | string   | no        | true       |
| period        | Period          | The period for which the benefit has been measured       | string   | no        | true       |
| modifiedDateTime| Modified DateTime | The most recent time that the Data Product Benefit was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true  |

