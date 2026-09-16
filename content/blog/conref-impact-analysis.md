---
title: "Conref Impact Analysis Before the Change"
slug: "conref-impact-analysis"
category: "DITA"
status: "draft"
description: "What reliable impact analysis should reveal before shared DITA content is modified."
---

# Conref Impact Analysis Before the Change

The cheapest time to understand the consequences of a shared-content change is before it is checked in. After publication or localization, discovery becomes a coordination problem.

## Direct use is only the beginning

A fragment may be reached through conkeyref, map inclusion, or another reused topic.

## Content state matters

Current work, approved baselines, and active translations can contain different revisions and therefore different impact sets.

## Results need classification

Authors should distinguish direct reuse, contextual resolution, historical inclusion, and unresolved references.

## Impact should guide review

ForgeDITA is designed to expose relationship evidence so reviewers can target affected publications rather than relying on blanket approvals.

## What to verify

Test the behavior with more than a base topic and one root map. Use specialized elements, alternate map contexts, scoped keys, direct and indirect reuse, controlled values, filtering, missing targets, and conflicting definitions. Inspect whether the editor, server validation, graph, search, and published output reach the same conclusion and whether the system can explain that conclusion.

## The operational consequence

DITA semantics are valuable because they let organizations manage complex content deliberately. When those semantics are only partly modeled, teams inherit plausible but inconsistent behavior. A strong CCMS makes the relevant context visible and keeps unsupported combinations outside its claim boundary until representative fixtures demonstrate them.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
