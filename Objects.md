# Objects

Objects are the core logical components of data storage as captured as part of the Analytics Design lifecycle.   



## ADML Objects

| Name               | Description                                                  | Originating Design Ritual |
| ------------------ | ------------------------------------------------------------ | ------------------------- |
| processArea        | A functional area or capability of an organisation.          | Information Design        |
| imperative         | An overarching theme for a set of related improvement objectives. | Information Design        |
| persona            | The stakeholders of a particular imperative who will ultimately will be consumers of a data product. | Information Design        |
| measurement        | A derived measure that supports monitoring and evaluation of performance. | Information Design        |
| activity           | An event or series of events that occur as part of a business process. | Information Design        |
| entity             | An object that participates or is created as part of a business process. | Information Design        |
| resource           | A person or technology which records data.                   | Information Design        |
| issue              | An existing or potential problem affective process imperatives and the ability to achieve goals. | Hypothesis Design         |
| outcomeChange      | The desired change in an outcome that will result from the issue being successfully addressed. | Hypothesis Design         |
| driver             | The variables that are related to the outcome change.        | Hypothesis Design         |
| intervention       | The things we can change to bring about an outcome change.   | Hypothesis Design         |
| dataProduct        | A configuration of data that can be consumed to solve a particular problem. | Hypothesis Design         |
| dataReadiness      | Validation of whether data exists in a form that will support the analytics objectives. | Data Readiness            |
| dataProductBenefit | Tracking of benefits of a data product over time.            | Learning                  |
| learning           | The documented findings from a learning review session.      | Learning                  |



## Object Properties 

| Name             | DisplayName       | Description                                                  | DataType           | Required? | Predefined |
| ---------------- | ----------------- | ------------------------------------------------------------ | ------------------ | --------- | ---------- |
| name             | Name              | The name of the object for technical reference and coding purposes | string             | yes       | yes        |
| description      | Description       | The description of the object                                | string             | yes       | yes        |
| version          | Version           | The **model** version that the object definition is based on | string             | yes       | yes        |
| modifiedDateTime | Modified DateTime | The most recent time when the object was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601). | datetimeoffset     | yes       | no         |
| customProperties | Custom Properties | Array of optional object properties - non-essential key/value pairs that contain contextual information that can be used to store additional context. | customProperties[] | no        | no         |



## Object Attributes 

Each attribute in an object has the following properties defined in the schema.

| Property    | Description                                                  |
| ----------- | ------------------------------------------------------------ |
| name        | The name of the attribute.                                   |
| displayName | The formatted display name of the attribute.                 |
| description | The description of the attribute.                            |
| dataType    | The data type expected.                                      |
| required?   | Whether the attribute must have a value as part of an array  |
| isNullable  | Whether an attribute can have a null value as part of an array |



## Custom Properties

Array of optional object properties - non-essential key/value pairs that contain contextual information that can be used to store additional context. Custom Properties are applied at model level about the object.

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





## Custom Attributes

Array of custom object attributes - non-essential key/value pairs that contain custom fields that can be used to store additional data. 
Custom Attributes are applied within the object to extend the information able to be stored alongside pre-defined attributes.

| Property | Type   | Description                   | Required? |
| :------- | :----- | :---------------------------- | :-------- |
| name     | string | Name of the Custom Attribute  | Yes       |
| value    | string | Value of the Custom Attribute | No        |

Example below:

```json
{
   "customAttributes":[
      {
         "name":"Owner",
         "value":"John Smith"
      }
   ]
}




```

