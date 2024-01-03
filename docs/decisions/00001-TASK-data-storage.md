---
# Configuration for the Jekyll template "Just the Docs"
parent: Decisions
nav_order: 100
title: Data Storage

# These are optional elements. Feel free to remove any of them.
# status: "{proposed | rejected | accepted | deprecated | … | superseded by [ADR-0005](0005-example.md)}"
# date: {YYYY-MM-DD when the decision was last updated}
# deciders: {list everyone involved in the decision}
# consulted: {list everyone whose opinions are sought (typically subject-matter experts); and with whom there is a two-way communication}
# informed: {list everyone who is kept up-to-date on progress; and with whom there is a one-way communication}
---
# Use a relational SQL database to store the data for the Attendance Register System

## Context and Problem Statement

It is necessary to decide how to store data that will be used by the Register Attendance System. For example, local vs cloud storage,
relational vs non-relational etc. This decision document will list the decisions made with regard to data storage and processing.

## Decision Drivers

* Ease of access - how easy it is to get specific data needed by the users of the system
* Speed - how fast users can access the data and how efficiently this is processed when data is changed
* Cost - hoe expensive it is to create and manage the database

## Considered Options

* Relational Database - SQL
* Non-relational database - NoSQL

## Decision Outcome

Relational SQL Database, because it is more effective when dealing with several distinct entities that have tangential relations to each other.
For example, rooms are not directly connected to a course, but a course has modules which then have a room assigned to them.
A relational database will provide the accuracy and ease of use when requesting complex data
A non-relational database may also work, however would have some limitations with regard to speed and ease of access of data

### Consequences

* Good, because a relational database can be created with specific identified entities, such as:
  - Students
  - Staff
  - Courses
  - Modules
  - Units
  - Rooms
  - Attendance
  - Grades
  - Classes
* Good, because data relation itegrity is enforced, so data cannot become as easily obsolete and therefore is more accurate and fit for
purpose
* Bad, as this can be more expensive than the alternative option

<!-- This is an optional element. Feel free to remove. -->
### Confirmation

{Describe how the implementation of/compliance with the ADR is confirmed. E.g., by a review or an ArchUnit test.
 Although we classify this element as optional, it is included in most ADRs.}

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

Entity Relation Database can be found here: {insert link to ERD here}
