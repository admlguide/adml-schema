# ADML Schema

### Schema definition

ADML is defined as a JSON schema that can be implemented in a range of platforms.

The core concepts in the JSON schema are:

- Objects;
- Attributes, 
- Relationships; and
- Bridges.

#### Objects

An object is a collection of attributes that represents a concept in the design process (e.g., hypothesis). [Custom objects](#extensions-and-tools) can be created to extend the logical model.

#### Attributes

Attributes are the fields within an object or bridge that correspond to data values within the data file. For example, a `Hypothesis` object may have attributes such as `HypothesisID` and `HypothesisName`. Custom attributes can be added to any object.

#### Relationships

Relationships are a logical definition of how objects are connected, such as a `Imperative:ImperativeID` joins to `Process Area:ImperativeID`.

Relationships are always assumed to be one-to-many, and generally use a foreign key relationship.

#### Bridges

Bridges provide a physical schema object to resolve many-to-many relationships.  

#### Entity relationship diagram

This entity relationship diagram provides a summary of all of the objects in ADML and how they are related.

|               ADML entity relationship diagram               |
| :----------------------------------------------------------: |
| ![img](https://documents.lucid.app/documents/4c72abb9-558c-40a0-a7d1-7f266d40a1a4/pages/9mqflgIV6CRU?a=12944&x=575&y=-2806&w=2750&h=1954&store=1&accept=image%2F*&auth=LCA%2084a2aa9beccc96d797f10d60e9401fc86c83526b-ts%3D1643265256) |

### ADML example

Shown below for illustrative purposes is an excerpt from an ADML JSON file.

```json
{
  "schema": "ADML",
  "schemaVersion": 1.0,
  "schemalocation": "github......"
  "name": "ADML for Organisation A",
  "description": "Organisation A's Enterprise Design Catalogue",
  "version": "1.2",
  "object":[
      {"name":"activity", "description":"An event or series of events that occur as part of a business process.", "version":"1.0"}
            ],
  "objectattributes":[
      {"name":"activityID", "DisplayName":"The unique identifier of the Activity", "DataType":"string","Required?":"yes","isNullable":"false"}
            ],
  "activity": [
"      {"activityID": "1, activityName:"Sales Pipeline"},
      {"activityID":"2,"activityName:"Order Fulfillment"}"
             ]
}


```



## Custom extensions and tools

### Custom properties and attributes

ADML has been designed to be inclusive rather than prescriptive. It allows for user customisation and extension in those areas where it would not be feasible to enumerate all the possibilities an organisation may have.

Extensions can be to:

- An object’s properties

- Attributes within an object

  

  To manage these customisations, the JSON schema has a concept of a **model** which allows an organisation to track versions of these customisations independently of the JSON schema version. 

  

  The following example demonstrates a customised property:

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

### Custom objects

Whilst the ADML schema is strict about the semantics to conform to the design methodology, it can theoretically be extended to include other objects to extend the schema further. Adherence to the standard properties of an object is recommended to ensure consistency across an organisation’s ADML **model**. We strongly encourage the community to contribute their innovation so future versions may include learnings across a number of implementations.