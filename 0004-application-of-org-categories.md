# 4. Application of Org Categories

Date: 26/06/2025 14:40

## Status

ACCEPTED

## Context

The application and standardization of the local Org Mode categorical indexing system across all org mode files.

## Decision

This ADR defines the context in which org mode "categories" should be understood. Furthermore it standardizes which
categories should be employed.

Categories should be understood to reflect the "category type" of the org mode node entry itself, and not about what the
node is referring to or what activity might be involved in the referring node. Therefore, in a time management based
system there are four primary categories, they are "tasks", "projects", "habits", and "events".

Events are the easiest to define, as they involve a specific point in time usually when an individual has to be present
at a specific location, or involved in performing a specific task. 

Tasks are a little less clear in definition, as they can involve a specific point and place in time, and can involve
performing a rather specific task. The distinguishment being the presence of accomplishment, as tasks are something that
need to be accomplished to obtain a specific goal or a conclusion of completedness.

Projects are really nothing more than a collection of tasks aimed at a common goal or larger task. Much like tasks
they have start times, deadlines, status updates, priorities, and effort estimates. In org mode there is some ambiguity
distinguishing between tasks and projects only because projects possess all the same characteristics as tasks. Yet, their
identity can be easily seen due to their possession of subtasks. In org mode, projects can have an infinite amount of
subprojects.

Habits can be difficult to define, due to their close similarity to tasks. Their defining characteristic is they have a
high frequency of recurrence due to their purpose, which is to reinforce the establishment of new personal behaviors.

## Consequences

Any time criteria is defined and standardized their is a loss of opportunity in what else could have been used in it’s place. 

