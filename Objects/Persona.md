# Persona

The stakeholders of a particular imperative who will ultimately will be consumers of a data product.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | persona                                                      |
| description | The stakeholders of a particular imperative who will ultimately will be consumers of a data product. |
| version     | 1.0                                                          |

## Attributes 

| Name         | DisplayName   | Description                                                  | DataType | Required? | isNullable |
| ------------ | ------------- | ------------------------------------------------------------ | -------- | --------- | ---------- |
| personaID    | Persona ID    | The unique identifier of the Persona                         | string   | yes       | false      |
| personaName  | Persona Name  | The name of the group of stakeholders                        | string   | yes       | false      |
| personaType  | Persona Type  | The categorisation of the type of stakeholder according to standard archetypes. | string   | no        | true       |
| imperativeID | imperative ID | The related imperative that the persona is a stakeholder of. | string   | yes       | false      |
| modifiedDateTime| Modified DateTime | The most recent time that the Persona was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no        | true   |

## Attribute Reference Data

| Name            | Value                 | Description                                                  |
| --------------- | --------------------- | ------------------------------------------------------------ |
| personaType | Sponsor | A stakeholder who is ultimately accountable for an outcome |
| personaType | Optimiser  | An agent that is responsible for identifying improvements in order to achieve a particular outcome. |
| personaType | Implementer | An agent that is responsible for taking action in the business process. |



