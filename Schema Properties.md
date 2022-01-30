# Schema Properties

The ADML JSON Schema consists of the following key concepts:

- The default **schema** definition covering:
  - Objects
  - Attributes within objects
  - Bridges

- An organisation’s own specific **model** implementation of ADML which may contain:
  - Custom **Properties** of Objects or Bridges
  - Custom **Attributes** of Objects or Bridges
  - Custom Objects

|           Overview of key concepts in ADML Schema            |
| :----------------------------------------------------------: |
| ![img](https://documents.lucid.app/documents/4c72abb9-558c-40a0-a7d1-7f266d40a1a4/pages/dHmNJfV-~DcX?a=13041&x=1765&y=-3857&w=1650&h=1244&store=1&accept=image%2F*&auth=LCA%205f031a4e8fc64e2e2bc89127ed2f2f016933e27d-ts%3D1643265256) |



## ADML Schema Properties

| Name        | DisplayName | Value                                                        | DataType | Required? | Predefined |
| ----------- | ----------- | ------------------------------------------------------------ | -------- | --------- | ---------- |
| name        | Name        | ADML                                                         | string   | yes       | yes        |
| description | Description | Analytics Design Markup Language                             | string   | yes       | yes        |
| author      | Author      | Nadav Rayman and Dr James Pearce                             | string   | yes       | yes        |
| version     | Version     | 1.0                                                          | string   | yes       | yes        |
| licence     | Licence     | ADML is licensed under the [Creative Commons Attribution-NoDerivatives 4.0 International](https://creativecommons.org/licenses/by-nd/4.0/legalcode) | string   | yes       | yes        |



## Model Properties 

| Name             | DisplayName       | Description                                                  | DataType           | Required? | Predefined |
| ---------------- | ----------------- | ------------------------------------------------------------ | ------------------ | --------- | ---------- |
| name             | Name              | The name of the model for technical reference and coding purposes | string             | no        | no         |
| description      | Description       | The description of the model                                 | string             | no        | no         |
| version          | Version           | The **model** version                                        | string             | no        | no         |
| schema           | Schema            | ADML                                                         | string             | yes       | yes        |
| schemaVersion    | Schema Version    | 1.0                                                          | string             | yes       | yes        |
| schemaLocation   | Schema Location   | Location of ADML JSON schema                                 | string             | yes       | yes        |
| modifiedDateTime | Modified DateTime | The most recent time when the object was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601). | datetimeoffset     | no        | no         |
| customProperties | Custom Properties | Array of optional object properties - non-essential key/value pairs that contain contextual information that can be used to store additional context. | customProperties[] | no        | no         |



## Custom Properties

Array of optional model properties - non-essential key/value pairs that contain contextual information that can be used to store additional context. Custom Properties are applied at model level about the object.

| Property | Type   | Description                  | Required? |
| :------- | :----- | :--------------------------- | :-------- |
| name     | string | Name of the Custom Property  | Yes       |
| value    | string | Value of the Custom Property | No        |



Example below:

```json
{
   "customProperties":[
      {
         "name":"ApprovedDate",
         "value":"20220101"
      }
   ]
}




```







