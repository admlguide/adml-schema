# Activity-Entity Relationship Description

Captures the description of the relationship between an Activity and an Entity, for a particular direction of relationship.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | activity-entityRelationshipDescription                       |
| description | Captures the description of the relationship between an Activity and an Entity, for a particular direction of relationship. |
| version     | 1.0                                                          |

## Attributes 

| Name         | DisplayName   | Description                           | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------- | -------- | --------- | ---------- |
| activityEntityRelationshipID | Activity Entity Relationship ID | The unique identifier for the relationship description | string | yes | false |
| activityID   | Activity ID   | The unique identifier of the Activity | string   | yes       | false      |
| entityID | Entity ID | The unique identifier of the Entity                          | string   | yes       | false      |
| relationshipDescription | Relationship Description | A brief description of an action that typically occurs between the Entity and Activity. | string | yes | false |
| descriptionFromID | Description From ID | Indicates whether the “ActivityID” or “EntityID” is the first subject in the action. | string | no | true |
| descriptionToID | Description To ID | Indicates whether the “EntityID” or the “ActivityID” is the second subject in the action. | string | no | true |
| modifiedDateTime             | Modified DateTime               | The most recent time that the item was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601). | datetimeoffset | no        | true       |
