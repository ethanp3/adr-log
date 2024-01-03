---
parent: Decisions
nav_order: 0
title: Data Storage

# These are optional elements. Feel free to remove any of them.
# status: "{proposed | rejected | accepted | deprecated | … | superseded by [ADR-0005](0005-example.md)}"
# date: {YYYY-MM-DD when the decision was last updated}
# deciders: {list everyone involved in the decision}
# consulted: {list everyone whose opinions are sought (typically subject-matter experts); and with whom there is a two-way communication}
# informed: {list everyone who is kept up-to-date on progress; and with whom there is a one-way communication}
---
# Use a Relational SQL database to store the data for the Advanced Foreign Services (AFS) Visa Processing System

## Context and Problem Statement

It is necessary to decide how to store data that will be used by the Visa Processing System. For example, local vs cloud storage,
Relational vs Non-Relational etc. This decision document will list the decisions made with regard to data storage and processing.

## Decision Drivers

* Ease of access - how easy it is to get specific data needed by the users of the system
* Speed - how fast users can access the data and how efficiently this is processed when data is changed
* Cost - hoe expensive it is to create and manage the database

## Considered Options

* Relational Database - SQL - PostgreSQL, Microsoft SQL Server, etc.
* Non-relational database - NoSQL - MongoDB etc.

## Decision Outcome

The system will use a relational SQL Database, as it is more effective when dealing with several distinct entities that have related data.
For example, all applications are directly connected to a user, and these can then have support tickets assigned to them, creating another link.
A relational database will provide the accuracy and ease of use when requesting complex data.
A non-relational database may also work, however would have some limitations with regard to speed and ease of access of data.

### Consequences

* Good, because a relational database can be created with specific identified entities, such as:
	- Users
	- Applications
	- Documents
	- Staff
* Good, because data relation itegrity is enforced, so data cannot become as easily obsolete and therefore is more accurate and fit for
purpose
* Bad, as this can be more expensive and restrictive than the alternative option if expanding the scope and structure of the database.

## Pros and Cons of the Options

### Relational SQL Database

* Good, because data relational integrity is enforced
* Good, because it is easier to access complex, related data
* Bad, because because as data builds up over time, queries may become slower due to the amount of data being processed
* Bad, because it can be more costly to run and manage

### Non-relational NoSQL Database

* Good, because it is cheaper than the alternative
* Good, because it can handle larger datasets
* Bad, because complex queries and data relations are not managed by this type of system well

## More Information

Entity Relation Database can be found included in the Task 1 Submission to show how the database may be structured
