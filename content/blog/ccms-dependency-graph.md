---
title: "The CCMS Dependency Graph: From File Storage to Content Infrastructure"
slug: "ccms-dependency-graph"
category: "Architecture"
status: "published"
published: "2026-09-03"
description: "Why maps, keys, conrefs, subject schemes, and reuse relationships require a contextual dependency graph rather than file-oriented storage alone."
---

# The CCMS Dependency Graph: From File Storage to Content Infrastructure

A DITA repository can store every file correctly and still misunderstand the content. DITA meaning emerges from relationships: maps establish context, keys resolve through scopes, conrefs reuse elements, subject schemes constrain values, and filters alter the effective publication.

## Relationships are first-class content

A file server can tell you that a topic exists. A graph-aware CCMS can tell you which maps use it, which topics reuse a fragment, where a key is defined, and which approved releases contain a particular revision. Those answers affect authoring, review, localization, and release decisions.

## Context changes the answer

A key name can resolve differently in two maps. A reference that is valid in one branch or profile may be absent in another. Resolution results therefore need to be associated with map context, content state, and relevant filtering inputs. Global lookup tables create answers that look definite while ignoring the conditions that made them true.

## Impact analysis must be explainable

Before changing shared content, a practitioner should be able to see inbound and outbound relationships and understand why each affected publication appears. Graph edges need provenance: source revision, target expression, semantic role, and resolution status. A list without that evidence is difficult to trust.

## The graph supports more than publishing

Validation can detect missing or ambiguous references, search can find reuse instead of matching text alone, and release comparison can explain changes in effective dependencies. ForgeDITA treats the graph as shared infrastructure so editors, validators, search, and publishing do not invent separate interpretations.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
