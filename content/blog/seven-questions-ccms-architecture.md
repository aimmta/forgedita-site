---
title: "Seven Questions That Expose a CCMS Architecture"
slug: "seven-questions-ccms-architecture"
category: "Evaluation"
status: "draft"
description: "Architecture questions for evaluating data ownership, semantic consistency, tenant isolation, reproducibility, and failure behavior."
---

# Seven Questions That Expose a CCMS Architecture

Feature lists compare visible functions. Architecture questions reveal who owns the content, where behavior lives, and how the platform changes under operational pressure.

## Where is the authoritative content representation?

Ask whether native XML is stored or reconstructed.

## Where are semantics declared?

Look for one inspectable model rather than private interpretations across services.

## What exactly identifies a release?

Content, processor, profile, and artifacts should be connected.

## How is tenant processing isolated?

Storage separation alone does not prevent shared toolchain drift.

## Can every client use the same APIs?

Editor integrations should not possess private platform powers.

## How does the system report uncertainty?

Partial and unavailable results must not appear successful.

## What does leaving require?

The answer should include content and processing assets before professional services are discussed.

## Require observable evidence

Do not settle for a verbal description when the platform can demonstrate the behavior. Ask for an API response, manifest, exported package, audit event, diagnostic record, or reproducible comparison. Capture the exact version and environment used in the evaluation so a successful result cannot later be attributed to a different configuration.

## Evaluate the operating life

Selection teams naturally focus on implementation and initial authoring. Extend the scenario to year three: a toolchain upgrade, a new specialization, a departed administrator, a regulatory inquiry, a migration, and an old release that must be rebuilt. A platform that handles those moments clearly will usually cost less organizational energy than one with a longer feature list.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
