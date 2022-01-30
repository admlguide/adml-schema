# Data Product-Item Bridge

Associates Objects to Data Products.

## Properties

| Property    | Value                                |
| ----------- | ------------------------------------ |
| name        | dataProduct-Item                     |
| description | Associates Objects to Data Products. |
| version     | 1.0                                  |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullableda |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| dataProductID    | Data Product ID | The unique identifier of the Data Product | string   | yes       | false      |
| itemType         | Item Type | Indicates which Object to link to | string   | yes       | false      |
| itemID           | Item ID | The unique identifier of the object being linked to | string | yes | false |
| modifiedDateTime| Modified DateTime | The most recent time that the item was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).  | datetimeoffset | no      | true   |
