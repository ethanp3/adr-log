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
# Use LaravelPHP and Livewire as the framework for the Attendance Record System

## Context and Problem Statement

Decide which programming language and framework to use for the Attendance Record System

## Considered Options

* Basic website - HTML, CSS, JavaScript etc (No Framework)
* MERN Stack - MongoDB, Express, React, NodeJS
* LaravelPHP and LiveWire

## Decision Outcome

Chosen option: LaravelPHP and Livewire, because it is the better option for development as it provides the flexibilty needed by the system.


{justification. e.g., only option, which meets k.o. criterion decision driver | which resolves force {force} | … | comes out best (see below)}.

### Consequences

* Good, as I have some experience with this framework and support available
* Bad, as it is not as popular of a framework so there is not as many resources available online

<!-- This is an optional element. Feel free to remove. -->
### Confirmation

{Describe how the implementation of/compliance with the ADR is confirmed. E.g., by a review or an ArchUnit test.
 Although we classify this element as optional, it is included in most ADRs.}

<!-- This is an optional element. Feel free to remove. -->
## Pros and Cons of the Options

### LaravelPHP and Livewire

<!-- This is an optional element. Feel free to remove. -->
{example | description | pointer to more information | …}

* Good, because it is very customisable
* Good, because it is easy to use
* Good, because it is secure. Useful when dealing with personal details
<!-- use "neutral" if the given argument weights neither for good nor bad -->
* Neutral, because it is not considered as popular as other frameworks such as React etc.
* Bad, because PHP is not as commonly used and there are fewer PHP developers. 


### MERN Stack - MongoDB, Express, React, Node

{example | description | pointer to more information | …}

* Good, because {argument a}
* Good, because {argument b}
* Neutral, because MongoDB is not a relational database, so not as consistent and less referential integrity than standard SQL databases
* Bad, because {argument d}
* …

<!-- This is an optional element. Feel free to remove. -->
## More Information

{You might want to provide additional evidence/confidence for the decision outcome here and/or
 document the team agreement on the decision and/or
 define when/how this decision should be realized and if/when it should be re-visited.
Links to other decisions and resources might appear here as well.}
