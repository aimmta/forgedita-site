---
title: "Map Context Is Not Optional for Correct Key Resolution"
slug: "map-context-key-resolution"
category: "DITA"
status: "draft"
description: "Why DITA key resolution belongs to a named map context and content state rather than a global lookup table."
---

# Map Context Is Not Optional for Correct Key Resolution

A key is not a global variable. Its effective definition depends on map context, scope, processing state, and sometimes filtering. Removing that context produces convenient but potentially incorrect answers.

## The same name can mean different things

Product variants and publication families can define one key differently without conflict because the maps establish separate contexts.

## Resolution belongs to a snapshot

A result should identify the map, relevant revisions, key definition, scope, and resolution status.

## Editors need the same answer as publishing

Local assistance becomes dangerous when it resolves against a different context than the server build.

## Context must remain inspectable

ForgeDITA persists context-aware results so a user can see what resolved, why it resolved, and which state produced the answer.

## What to verify

Test the behavior with more than a base topic and one root map. Use specialized elements, alternate map contexts, scoped keys, direct and indirect reuse, controlled values, filtering, missing targets, and conflicting definitions. Inspect whether the editor, server validation, graph, search, and published output reach the same conclusion and whether the system can explain that conclusion.

## The operational consequence

DITA semantics are valuable because they let organizations manage complex content deliberately. When those semantics are only partly modeled, teams inherit plausible but inconsistent behavior. A strong CCMS makes the relevant context visible and keeps unsupported combinations outside its claim boundary until representative fixtures demonstrate them.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
