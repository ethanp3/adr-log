---
# Configuration for the Jekyll template "Just the Docs"
parent: Decisions
nav_order: 100
title: ADR Template

# These are optional elements. Feel free to remove any of them.
# status: "{proposed | rejected | accepted | deprecated | … | superseded by [ADR-0005](0005-example.md)}"
# date: {YYYY-MM-DD when the decision was last updated}
# deciders: {list everyone involved in the decision}
# consulted: {list everyone whose opinions are sought (typically subject-matter experts); and with whom there is a two-way communication}
# informed: {list everyone who is kept up-to-date on progress; and with whom there is a one-way communication}
---
# Use MERN as the technology stack for the Advanced Foreign Services (AFS) Visa Processing System

## Context and Problem Statement

Decide which framework and technology stack to use for the Advanced Foreign Services (AFS) Visa Processing System

## Considered Options

* Basic website - HTML, CSS, JavaScript etc. (No Framework)
* MERN Stack - MongoDB, Express, React, NodeJS
* MEAN Stack - MongoDB, Express, Angular, NodeJS
* LAMP Stack - Linux, Apache, MySQL, PHP

## Decision Outcome

Chosen option: MERN Stack. This provides the stability and flexibility that the system needs. 


**{justification. e.g., only option, which meets k.o. criterion decision driver | which resolves force {force} | … | comes out best (see below)}.

### Consequences

* Good, as this is is a widely accepted and used tech stack, with lots of support available. Likely to be supported for a long time and 
many existing large-scale systems also use this solution.
* Bad, as it requires a lot of varied technical knowledge to be able to use, create, and modify each element of the system. 

<!-- This is an optional element. Feel free to remove. -->
### Confirmation

{Describe how the implementation of/compliance with the ADR is confirmed. E.g., by a review or an ArchUnit test.
 Although we classify this element as optional, it is included in most ADRs.}

## Pros and Cons of the Options

### Basic website - HTML, CSS, JavaScript etc. (No framework)

* Good, because the learning curve for developers is less steep. Other technology stacks require knowledge of HTML, CSS, JavaScript and then
expand on these
* Good, because it is a more lightweight solution. Less resource intensive and less reliability on third-party tools and libraries
* Neutral, because it requires less code to create the project, but does not have the pre-existing structure and templates that a framework provides
* Bad, because it is not as efficient. Creating everything manually is not very time-efficient and might be harder to debug any issues that may arise

### MERN Stack - MongoDB, Express, React, Node

* Good, because it provides good performance, due to the simplicity of the MongoDB lack of relationships. Able to process high levels 
of data and requests concurrently
* Good, because it is a commonly used and accepted technology stack
* Good, because it is already used by similar large scale products and services
* Neutral, because MongoDB is not a relational database, so not as consistent and less referential integrity than standard SQL databases
* Bad, because ....

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

<!-- This is an optional element. Feel free to remove. -->
## More Information

{You might want to provide additional evidence/confidence for the decision outcome here and/or
 document the team agreement on the decision and/or
 define when/how this decision should be realized and if/when it should be re-visited.
Links to other decisions and resources might appear here as well.}
