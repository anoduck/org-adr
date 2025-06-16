# 5. Org Mode Agenda File Layout

Date: 16/06/2025 02:41

## Status

ACCEPTED

## Context

While Org Mode files can be arranged in an infinite number of layouts, this absence of structure is not desired for org
files whose purpose is to record and maintain a working list of projects and tasks. In fact, due to other features such
as org-captures and refiling, it is best to maintain a uniform structure.

The files used to maintain a running list of projects and tasks is referred to as Org Agenda Files, because they are
processed to generate the org-agenda.

## Decision

After the Header is provided, there shall be at least two first level headings:

1. Tasks
2. Projects

## Consequences

This might limit the robustness of using the org-file for tracking complex projects, but it is rather doubtful.
