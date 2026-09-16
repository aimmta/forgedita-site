---
title: "Why XML Grammars Cannot Carry All Operational Semantics"
slug: "xml-grammars-operational-semantics"
category: "DITA"
status: "draft"
description: "The separate roles of grammars, subject schemes, semantic registries, validation rules, and processor behavior."
---

# Why XML Grammars Cannot Carry All Operational Semantics

A grammar can define valid structure. It cannot by itself tell every service which relationships to extract, how specialized constructs behave operationally, or which metadata affects search and workflow.

## Structure and behavior are different

DTD, RNG, and XSD answer whether content fits a declared vocabulary. They do not form a complete processing contract.

## Scattered meaning creates drift

When editors, validators, graph services, and transforms hardcode meaning separately, specialized content receives inconsistent treatment.

## Declare cross-service roles

A semantic registry can map DITA classes and specialized elements to reference, reuse, taxonomy, filtering, or policy roles.

## Keep each tool honest

The registry does not replace grammars or subject schemes. It coordinates operational meaning while those standards retain their own responsibilities.

## What to verify

Test the behavior with more than a base topic and one root map. Use specialized elements, alternate map contexts, scoped keys, direct and indirect reuse, controlled values, filtering, missing targets, and conflicting definitions. Inspect whether the editor, server validation, graph, search, and published output reach the same conclusion and whether the system can explain that conclusion.

## The operational consequence

DITA semantics are valuable because they let organizations manage complex content deliberately. When those semantics are only partly modeled, teams inherit plausible but inconsistent behavior. A strong CCMS makes the relevant context visible and keeps unsupported combinations outside its claim boundary until representative fixtures demonstrate them.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
