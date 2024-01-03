---
parent: Decisions
nav_order: 0
title: Framework and Tech Stack

# These are optional elements. Feel free to remove any of them.
# status: "{proposed | rejected | accepted | deprecated | … | superseded by [ADR-0005](0005-example.md)}"
# date: {YYYY-MM-DD when the decision was last updated}
# deciders: {list everyone involved in the decision}
# consulted: {list everyone whose opinions are sought (typically subject-matter experts); and with whom there is a two-way communication}
# informed: {list everyone who is kept up-to-date on progress; and with whom there is a one-way communication}
---
# Use PERN as the technology stack for the Advanced Foreign Services (AFS) Visa Processing System

## Context and Problem Statement

Decide which framework and technology stack to use for the Advanced Foreign Services (AFS) Visa Processing System

## Considered Options

* Basic website - HTML, CSS, JavaScript etc. (No Framework)
* PERN Stack - PostgreSQL, Express, React, NodeJS
* MERN Stack - MongoDB, Express, React, NodeJS
* MEAN Stack - MongoDB, Express, Angular, NodeJS
* LAMP Stack - Linux, Apache, MySQL, PHP

## Decision Outcome

Chosen option: PERN Stack. This provides the stability and flexibility that the system needs, with a modern framework and open-source relational database

### Consequences

* Good, as this is is a widely accepted and used tech stack, with lots of support available. Likely to be supported for a long time and 
many existing large-scale systems also use this solution
* Bad, as it requires a lot of varied technical knowledge to be able to use, create, and modify each element of the system

### Confirmation

* Unit Testing and Integration Testing will be carried out to ensure the product serves its purpose and to identify any bugs or errors prior to live deployment

## Pros and Cons of the Options

### Basic website - HTML, CSS, JavaScript etc. (No framework)

* Good, because the learning curve for developers is less steep. Other technology stacks require knowledge of HTML, CSS, JavaScript and then
expand on these
* Good, because it is a more lightweight solution. Less resource intensive and less reliability on third-party tools and libraries
* Neutral, because it requires less code to create the project, but does not have the pre-existing structure and templates that a framework provides
* Bad, because it is not as efficient. Creating everything manually is not very time-efficient and might be harder to debug any issues that may arise

### PERN Stack - PostgreSQL, Express, React, Node

* Good, because it uses JavaSCript throughout the project, reducing the need for developers to adapt to new environments and technologies
* Good, because the database is relational in structure, allowing easier data querying and data integrity
* Good, because it is able to scale up easily
* Neutral, because it is not as widely used as other stacks
* Bad, because it might require more specific knowledge not as many developers have

### MERN Stack - MongoDB, Express, React, Node

* Good, because it provides good performance, due to the simplicity of the MongoDB lack of relationships. Able to process high levels 
of data and requests concurrently
* Good, because it is a commonly used and accepted technology stack
* Good, because it is already used by similar large scale products and services
* Neutral, because MongoDB is not a relational database, so not as consistent and less referential integrity than standard SQL databases
* Bad, because the database is non-relational in structure

### MEAN Stack - MongoDB, Express, Angular, Node

* Good, because it provides good performance, due to the simplicity of the MongoDB lack of relationships. Able to process high levels 
of data and requests concurrently
* Good, because it is a commonly used and accepted technology stack
* Good, because it is already used by similar large scale products and services
* Neutral, because MongoDB is not a relational database, so not as consistent and less referential integrity than standard SQL databases
* Bad, because it can be directly compared with MERN stacks as they are very similar, only changing React to Angular. However, Angular
has less users and developers, so therefore less support and help with resources

### LaravelPHP and Livewire

* Good, because it is very customisable and easy to use for customers
* Good, because it is secure. Useful when dealing with personal, sensitive details
* Neutral, because it is not considered as popular as other frameworks such as React etc
* Bad, because PHP is not as commonly used and there are fewer PHP developers