# Relationships

Relationships are a logical definition of how objects are connected.

Relationships are always assumed to be one-to-many, and use a foreign key relationship.

To maintain simplicity of the model, **Bridges**, provide a physical schema object to resolve many-to-many relationships.



## ADML Schema Relationships 

| *(one item in)* Object | Related to *(many items in)* Object      | Related by                                                   |
| ---------------------- | ---------------------------------------- | ------------------------------------------------------------ |
| Process Area           | Imperative                               | ProcessID                                                    |
| Imperative             | Persona                                  | ImperativeID                                                 |
| Imperative             | Measurement                              | via Imperative-Measurement Bridge<br />MeasurementID & ImperativeID |
| Persona                | Measurement                              | via Persona-Measurement Bridge<br />PersonaID & ImperativeID |
| Imperative             | Hypothesis                               | ImperativeID                                                 |
| Hypothesis             | Issue                                    | HypothesisID                                                 |
| Issue                  | Outcome Change                           | IssueID                                                      |
| Outcome Change         | Driver                                   | OutcomeChangeID                                              |
| Driver                 | Intervention                             | DriverID                                                     |
| Driver                 | Data Product                             | via Data Product-Item Bridge<br />ItemID = DriverID where Item Type = “Driver” |
| Outcome Change         | Data Product                             | via Data Product-Item Bridge<br />ItemID = OutcomeChangeID where ItemType = “OutcomeChangeID” |
| Data Readiness         | Data Product                             | via Data Product-Item Bridge<br />ItemID = DataReadinessID where ItemType = “Data Readiness” |
| Resource               | Data Product                             | via Data Product-Item Bridge<br />ItemID = ResourceID where ItemType = “Resource” |
| Intervention           | Data Product                             | via Data Product-Item Bridge<br />ItemID = InterventionID where ItemType = “Intervention” |
| Measurement            | Activity                                 | via Activity-Measurement Bridge<br />ActivityID & MeasurementID |
| Activity               | Entity                                   | via Activity-Entity Bridge<br />ActivityID & EntityID        |
| Entity                 | Activity                                 | via Activity-Entity Bridge<br />ActivityID & EntityID        |
| Activity-Entity Bridge | Activity-Entity Relationship Description | ActivityID & EntityID <br />DescriptionFromID = “ActivityID” or “EntityID”<br />DescriptionToID=“EntityID” or “ActivityID” |
| Data Product           | Learning                                 | DataProductID                                                |
| Data Product           | Data Product Benefit                     | DataProductID                                                |



## Bridges

Bridges are typically used to relate objects that do not adhere to a single foreign key based one-to-many relationship.

| Name                                     | Description                                                  |
| ---------------------------------------- | ------------------------------------------------------------ |
| Activity-Measurement Bridge              | Associates a measurement with many activities                |
| Imperative-Measurement Bridge            | Associates an imperative with many measurements              |
| Persona-Measurement Bridge               | Associates a persona with many measurements                  |
| Activity-Entity Bridge                   | Associates activities and entities                           |
| Data Product-Item Bridge                 | Associates Resources, Drivers, Outcome Changes, Interventions, Data Readiness and Measurements to Data Products. It can be extended using its generic pattern to link to other objects also. |
| Activity-Entity Relationship Description | Captures the description of the relationship between an Activity and an Entity, for a particular direction of relationship. |



### Bridge Properties

| Name             | DisplayName       | Description                                                  | DataType           | Required? | Predefined |
| ---------------- | ----------------- | ------------------------------------------------------------ | ------------------ | --------- | ---------- |
| name             | Name              | The name of the bridge for technical reference and coding purposes | string             | yes       | yes        |
| description      | Description       | The description of the bridge                                | string             | yes       | yes        |
| version          | Version           | The model version that the bridge definition is based on     | string             | yes       | yes        |
| modifiedDateTime | Modified DateTime | The most recent time when the bridge was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601). | datetimeoffset     | yes       | no         |
| customProperties | Custom Properties | Array of optional bridge properties - non-essential key/value pairs that contain contextual information that can be used to store additional context. | customProperties[] | no        | no         |



## Custom Properties

Array of optional bridge properties - a non-essential key/value pairs that contain contextual information that can be used to store additional context. Custom Properties are applied at model level about the object.

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

Array of custom bridge attributes - a non-essential key/value pairs that contain custom fields that can be used to store additional data. 
Custom Attributes are applied within the bridge to extend the information able to be stored alongside pre-defined attributes.

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

