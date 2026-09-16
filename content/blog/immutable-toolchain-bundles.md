---
title: "Why Toolchain Bundles Must Be Versioned and Immutable"
slug: "immutable-toolchain-bundles"
category: "Publishing"
status: "published"
published: "2026-09-08"
description: "How immutable tenant toolchain bundles reduce publishing drift, isolate customers, and make historical releases rebuildable."
---

# Why Toolchain Bundles Must Be Versioned and Immutable

DITA publishing behavior does not come from DITA-OT alone. Plugins, catalogs, grammar shells, Schematron, themes, DITAVAL presets, parameters, and runtime policy all contribute to the output. If those inputs can change in place, a release cannot identify the environment that produced it.

## A bundle names the complete environment

A toolchain bundle should carry a manifest that identifies every governed processing asset and its version. Validation can reject missing dependencies before promotion. Once promoted, the bundle becomes immutable and later changes create a new version rather than altering the old one.

## Tenant scope prevents accidental coupling

One organization may require a regulated PDF plugin while another uses a different DITA-OT version and HTML theme. Shared mutable installations force coordination between unrelated customers. Tenant-scoped bundles allow those environments to evolve independently and make cross-tenant effects testable.

## Historical releases retain their processor

Content baselines are not enough when the transformation environment has moved on. Retaining the named bundle lets a release rebuild against the processing rules originally approved. The runtime manifest can then compare content, bundle, profile, and artifact fingerprints.

## Immutability is a lifecycle decision

Bundles still need upload, validation, promotion, deprecation, and retention rules. Immutability does not mean every candidate is permanent. It means an accepted release input cannot be silently rewritten. ForgeDITA makes that constraint explicit because stable history is more valuable than convenient mutation.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
