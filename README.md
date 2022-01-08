# Neo4j_units_degree_dataset
In this project, a graph is built representing units offered in a university and their relationships. Few queries are designed to show that the graph can
be used to check degree and unit rules.

The graph models:

•at least one degree (three or four year) with a set of completion requirements;

•enough units at 1000, 2000, and 3000 or above level to satisfy that degree’s completion requirements (there should be at least three or four units per level);

•some units with no prerequisites;

•some units with a list of prohibition units;

•some units with a list of prerequisite units linked by OR operators;

•some units with two or more prerequisite units linked by OR and AND operators;

•a chain of units linked by two or three prerequisite relationships.

The guide must contain the following slides:

• Slide one: Graph Building. In this slide, you should provide one or more queries to build a graph containing units, degrees, and their relationships. You should prepare
a data file containing units information and load that file to build a graph units information. You may write a separate query to add degree information. In the
textual description section of this slide, briefly describe the nodes and relationships in the graph.

• Slide two: Graph Inspection. In this slide, include some queries to show that your graph contains units with the following features:
– has no prerequisite
– has a prohibition list
– has a list of prerequisites units linked by OR operators
– has a list of prerequisites units linked by AND and OR operators

• Slide three: Prohibition Rule. In this slide, write a query to insert a student’s information in the graph. The student should have one basic property such as a name and
should have completed some units. Write a query to check if the student is allowed to enrol in a unit based on its prohibition rule. You should prepare two unit codes:
one that satisfies the prohibition rule and one that does not satisfy the rule. The unit codes to be used should be included in the textual description part of this slide.

• Slide four: Prerequisite Rule. This slide also needs a student’s information. You may reuse the one added in slide three if appropriate. Otherwise, write a query to insert
another student’s information in the graph. The student should have completed some units. The units completed by the student should
– satisfy the prerequisites of a unit (A) with only OR linked prerequisites;
– satisfy the prerequisites of another unit (B) with both AND and OR linked prerequisites;
and
– does not satisfy the prerequisites of a third unit (C) with both AND and OR linked prerequisites.
You should prepare three unit codes that correspond to the above three units A, B and C, and include them in the textual description part of this slide. Write ONE
query to check the prerequisite rule. The query should have a default value to check the prerequisite of unit A. It should be able to check unit B and C by replacing the
unit code accordingly.

• Slide five: Graduation Checking. Insert another student’s information in the graph. This student should have completed the degree’s total credit points requirement but does not meet some level’s credit points requirements. Write a query to run the check
and print out a list of Boolean values, each representing the status of a rule.

• Slide six: Indirect Prerequisite. In this slide, write a query to find all 1000 level indirect prerequisite units of a given unit and print out the prerequisite chain from
the unit to the 1000 level indirect prerequisite unit. An indirect prerequisite unit could be one or more units away from the given unit in a prerequisite chain. You
should prepare two unit codes: one that has a maximum chain length of 2, the other has a maximum chain length of 3. The unit codes should be included in the textual
description of this slide.

• Slide seven: Foundational Unit. In this slide write a query to find the unit(s) appearing in most other unit’s direct or indirect prerequisite list. In the textual description
part, briefly describe the expected result of this query.

• Slide eight: Clear the Graph. In this slide write a query to delete all nodes and their
relationships in the graph.
