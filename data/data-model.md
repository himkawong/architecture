# Data Model

### First Normal Form (1NF)
* Each attribute contains only one value.
* All attribute values are atomic, which means they can’t be broken down into anything smaller.
### Second Normal Form (2NF)
* It is in 1NF.
* No non-prime attributes are functionally dependent on a subset of the candidate key(s). In other words, any column that’s not a key column is dependent on the whole information in the candidate key.

### Third Normal Form (3NF)
* It is in second normal form (2NF).
* All non-prime attributes are directly (non-transitively) dependent on the entire candidate key.

## Conceptual Data Model
* Purpose: define the scope of the solution. It also serves as a common ground for communicating and defining the business requirements, concepts, and rules.
* Output: a diagram (ER) with all of the main entities their relationships, and high-level attributes.
* Subject Area: 
  * Enable you to subdivide your model into separate logical groups or domains. Data modeling is an iterative process—even more so when using subject areas. 
  * Engage the business leaders and stakeholders to identify common subject areas.
  * Prioritize which subject areas should be addressed and when.
  * For each subject area, repeat the process of identifying entities, attributes, and relationships.

## Logical Data Model

* logical model is a conceptual model to which DATA NORMALIZATION TECHNIQUES have been applied and for which all of the attributes have been identified
* Relational Model vs Dimensional Model ?

## Physical Data Model

* All of the entities are transformed into tables and the attributes (i.e. columns) are associated with specific data types according to the target database engine

https://en.wikipedia.org/wiki/Data_modeling
https://vertabelo.com/blog/data-modeling-basics/
https://www.mongodb.com/resources/basics/databases/data-modeling
https://www.nitorinfotech.com/blog/data-modeling-standards-and-guidelines/
https://www.thoughtspot.com/data-trends/data-modeling/conceptual-data-model-examples

