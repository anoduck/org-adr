# 7. Org File Header

Date: 18/07/2025 06:08

## Status

ACCEPTED

## Context

1. Standardization of org file header
2. Org Mode system organization and configurable variables. 
3. Org File Header construction and definition.

Org Mode accepts configuration variables on both a global basis and a per file basis. Setting configuration variables
globally is done in either the configuration mode or in the configuration file, while configuration variables set on a
per file basis are kept within the header of the Org Mode file itself. Which means you can have four different files
open in the same session of Emacs, with four different configurations.

Configuration variables set within an Org Mode file are always prioritized over global configuration variable settings,
and some variables are only set on a per file basis.

## Decision

Due to the ability for individual org files to change the configuration of org mode, the org file header should be
standardized across all files within the org mode system, except where it is explicitly desired otherwise. 

Below is the header that should be used within our localized org system for all org mode agenda file entries.

```org
#+TITLE:
#+DATE:
#+DESCRIPTION:
#+PROJECT:
#+PROPERTY: Effort_ALL 0 0:10 0:30 1:00 2:00 3:00 4:00 5:00 6:00 7:00 8:00 10:00 12:00 18:00 24:00
#+TAGS: Home(h) Writing(w) Shooting(s) Phone(p) Computer(c) Project(a) Errands(e) Legal(l) Find(f) Farm(g) Financials(m)
#+PRIORITY: A B C D
#+OPTIONS: H:3 num:nil toc:nil \n:nil @:t ::t |:t ^:t -:t f:t *:t TeX:t LaTeX:nil skip:nil d:nil todo:t pri:nil tags:not-in-toc
#+EXPORT_SELECT_TAGS: EXPORT
#+EXPORT_EXCLUDE_TAGS: noexport
#+STARTUP: align nodlcheck nofold oddeven hidestars showall
#+DRAWERS: PROPERTIES CLOCK LOGBOOK RESULTS FEEDSTATUS LINK
#+COLUMNS: %38ITEM(Details) %TASKID %TAGS(Context) %7SCHEDULED(Planned) %7TODO(To Do) %5PRIORITY(PRIORITY) %5ESTIMATED{+} %3ACTUAL{+} %5DONE(Completeness){X%} %17Effort(Estimated Time){:} %6CLOCKSUM(Total){:}
# Start here =============================================================================
```

## Consequences

All decisions have good and bad consequences:

### Good

- Encourages uniformity across all org files in the system.
- Prevents rogue variables from existing
- Provides variables to system that can only be set on a per file basis.

### Bad 

- Limits Tag availability to a finite set.
- Not resistant to upstream changes in org mode
- Does increase processing time of org files.
