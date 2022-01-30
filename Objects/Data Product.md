# Data Product

A configuration of data that can be consumed to solve a particular problem.

## Properties

| Property    | Value                                                        |
| ----------- | ------------------------------------------------------------ |
| name        | dataProduct                                                  |
| description | A configuration of data that can be consumed to solve a particular problem. |
| version     | 1.0                                                          |

## Attributes 

| Name                | DisplayName           | Description                                                  | DataType | Required? | isNullable |
| ------------------- | --------------------- | ------------------------------------------------------------ | -------- | --------- | ---------- |
| dataProductID       | Data Product ID       | The unique identifier of a Data Product                      | string   | yes       | false      |
| dataProductName     | Data Product Name     | The name of the Data Product                                 | string   | yes       | false      |
| dataProductCategory | Data Product Category | The generic type of asset that the Data Product can be classified as as per listed example reference data. | string   | no        | true       |
| publishingMechanism | Publishing Mechanism  | The means by which the Data Product is published for use.    | string   | yes       | false      |
| approvedPurpose     | Approved Purpose      | The officially sanctioned business application of the Data Product. | string   | no        | true       |
| reliabilityRating   | Reliability Rating    | A rating of the reliability of the Data Product based on the governance processes which indicate the certifiability of results represented. | string   | no        | true       |
| sensitivityRating   | Sensitivity Rating    | A classification of sensitivity of data contents.            | string   | no        | true       |
| modifiedDateTime| Modified DateTime | The most recent time that the Data Product was updated in date time offset per [ISO 8601](https://www.wikipedia.org/wiki/ISO_8601).      | datetimeoffset | no      | true   |


## Attribute Reference Data

| Name            | Value                 | Description                                                  |
| --------------- | --------------------- | ------------------------------------------------------------ |
| dataProductCategory | Dashboard | A summary display of performance. |
| dataProductCategory | Report           | A specific list of cases or items requiring attention.       |
| dataProductCategory | Alert            | A message to indicate that a situation has exceeded a defined threshold. |
| dataProductCategory | Recommendation   | A real-time signal or message to take a course of action.    |
| dataProductCategory | What If Tool     | A display of projected performance based on parameter selection or input of different potential scenarios. |
| dataProductCategory | Predictive Model | An automated calculation of propensity or an estimate.       |
| dataProductCategory | Optimisation     | An automated configuration of decisions based on projected performance and pre-defined constraints. |
| publishingMechanism | API | Published as a live endpoint to enable application integration. |
| publishingMechanism | Application Embedded | Exposed in an existing application. |
| publishingMechanism | Visualisation Portal | Published to a portal to be able to accessed on-demand. |
| publishingMechanism | Desktop Tool | Available as a utility that is able to be run on existing desktop software, or installed as a standalone utility |
| publishingMechanism | Dataset | Published as a dataset for development of visualisations or as an input to further data processing and modelling. |
| approvedPurpose | Compliance |  |
| approvedPurpose | Operational |  |
| approvedPurpose | Strategic Planning |  |
| approvedPurpose | Exploratory |  |
| reliabilityRating | Gold | Data has been acquired from a trusted source, has automated data quality testing in place and has satisfied publishing standards to enable general business consumptions. |
| reliabilityRating | Silver | Data which has been acquired from a trusted source, is being intermittently monitored for data quality issues, and is in use by expert data practitioners. |
| reliabilityRating | Bronze | Data has been assembled in an experimental fashion as part of an exploratory phase to assess the utility of data long term. |
| sensitivityRating | Public | Business data that is specifically prepared and approved for public consumption. |
| sensitivityRating | General | Business data that is not intended for public consumption. However, this can be shared with external partners, as required. Examples include a company internal telephone directory, organizational charts, internal standards, and most internal communication. |
| sensitivityRating | Confidential | Sensitive business data that could cause damage to the business if shared with unauthorized people. Examples include contracts, security reports, forecast summaries, and sales account data. |
| sensitivityRating | Highly Confidential | Very sensitive business data that would cause damage to the business if it was shared with unauthorized people. Examples include employee and customer information, passwords, source code, and pre-announced financial reports. |



