---
title: "Why Feature Matrices Hide Operational Risk"
slug: "feature-matrices-hide-risk"
category: "Evaluation"
status: "draft"
description: "Why yes-or-no feature comparisons miss quality, scope, failure behavior, maintainability, and long-term cost."
---

# Why Feature Matrices Hide Operational Risk

A matrix can show that two platforms both have workflow, search, validation, APIs, and publishing. It cannot show whether those capabilities remain understandable under change.

## A checkmark hides scope

Search may mean filenames or contextual DITA relationships. Workflow may mean a state field or governed decisions.

## Quality appears in failure

The matrix rarely asks whether a timeout becomes partial, failed, or silently empty.

## Operations determine ownership cost

Upgrade isolation, observability, recovery, and export contracts shape years of work after selection.

## Use scenarios beside the matrix

Retain feature coverage, but require demonstrations, evidence, limitations, and operating assumptions for every material capability.

## Require observable evidence

Do not settle for a verbal description when the platform can demonstrate the behavior. Ask for an API response, manifest, exported package, audit event, diagnostic record, or reproducible comparison. Capture the exact version and environment used in the evaluation so a successful result cannot later be attributed to a different configuration.

## Evaluate the operating life

Selection teams naturally focus on implementation and initial authoring. Extend the scenario to year three: a toolchain upgrade, a new specialization, a departed administrator, a regulatory inquiry, a migration, and an old release that must be rebuilt. A platform that handles those moments clearly will usually cost less organizational energy than one with a longer feature list.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
