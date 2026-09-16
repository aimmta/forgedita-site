---
title: "What Specialization-Aware Processing Actually Requires"
slug: "specialization-aware-processing"
category: "DITA"
status: "draft"
description: "Why accepting specialized XML is not enough, and how class-based semantics must reach validation, graph, search, editors, and publishing."
---

# What Specialization-Aware Processing Actually Requires

A system can store a specialized topic without understanding it. Genuine specialization awareness means derived elements participate in the same semantics as their base classes unless an explicit extension says otherwise.

## Do not hardcode element names

Processing should use DITA class ancestry and domain declarations so customer vocabularies do not disappear from graph or validation behavior.

## Deliver the grammar assets

Catalogs, shells, constraints, templates, and author CSS must reach the editor and server from a governed bundle.

## Extend semantics explicitly

Tenant declarations should add specialized roles without patching each service independently.

## Test through the full path

A fixture should author, validate, resolve, search, publish, export, and re-import specialized content before broad support is claimed.

## What to verify

Test the behavior with more than a base topic and one root map. Use specialized elements, alternate map contexts, scoped keys, direct and indirect reuse, controlled values, filtering, missing targets, and conflicting definitions. Inspect whether the editor, server validation, graph, search, and published output reach the same conclusion and whether the system can explain that conclusion.

## The operational consequence

DITA semantics are valuable because they let organizations manage complex content deliberately. When those semantics are only partly modeled, teams inherit plausible but inconsistent behavior. A strong CCMS makes the relevant context visible and keeps unsupported combinations outside its claim boundary until representative fixtures demonstrate them.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
