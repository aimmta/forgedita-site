---
title: "How to Evaluate CCMS Publishing Reproducibility"
slug: "evaluate-publishing-reproducibility"
category: "Evaluation"
status: "draft"
description: "A practical reproducibility test covering content baselines, toolchains, profiles, manifests, and artifact comparison."
---

# How to Evaluate CCMS Publishing Reproducibility

Reproducibility should be tested, not inferred from version labels. A meaningful evaluation begins with two builds whose inputs are independently identified.

## Seal the content state

Use an immutable baseline containing exact revisions, not a mutable folder or branch name.

## Identify the complete processor

Pin the toolchain bundle, profile, filtering inputs, and relevant runtime policy.

## Compare structured evidence

Record manifests and artifact hashes, accounting explicitly for permitted nondeterministic metadata.

## Change one input

Verify that an intentional content or toolchain change creates a traceable fingerprint difference while unchanged inputs remain stable.

## Require observable evidence

Do not settle for a verbal description when the platform can demonstrate the behavior. Ask for an API response, manifest, exported package, audit event, diagnostic record, or reproducible comparison. Capture the exact version and environment used in the evaluation so a successful result cannot later be attributed to a different configuration.

## Evaluate the operating life

Selection teams naturally focus on implementation and initial authoring. Extend the scenario to year three: a toolchain upgrade, a new specialization, a departed administrator, a regulatory inquiry, a migration, and an old release that must be rebuilt. A platform that handles those moments clearly will usually cost less organizational energy than one with a longer feature list.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
