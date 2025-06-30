# 6. Org-Mode-todo-states

Date: 29/06/2025 15:20

## Status

ACCEPTED

## Context

Task states or colloquially referred to as task statuses. Also referred to as todo labeling.

## Decision

Task states are determined by personal preferrence, but regardless need to be established in order for org mode to
maintain proper functionality. Additionally, several org mode packages require the use of certain task states that are
outside the realm of normal convention. For these exceptionary instances we reccommend limiting their influence on the
org instance by defining task states in the org mode header.

Two task states are common across all instances of org no matter what they are labeled or who is using them, these
states are `TODO` and `DONE`. Sometimes they are labeled as `Open` and `Closed`, but the meaning is the same. One refers
to a state of completedness, and the other incompletedness. 

A third state not commonly found, but highly recommended, `canceled`. Which designates completion of the task was not
attempted, and there was no effort invested, and is an important distinction to make in task management.

A more common task state, which has grown in popularity for org mode instances, is `laters`. Often this is labeled as
`waiting`, but the use of the label is a misnomer primarily due to the fact the task is often not waiting on anything
other than for time to become available. 

There is also the use of `WAIT`, which we prefer to use the label `ONHOLD`, and this is because the task is held waiting
on some other task to become completed. 

## Consequences

If you employ numerous plugins that possess their own todo states that are a requirement, your agenda can become quite
messy, and refiling can be difficult to accomplish.
