---
title: "Why Validation Results Must Identify Their Sources"
slug: "validation-results-identify-sources"
category: "ForgeDITA"
status: "draft"
description: "Why useful validation diagnostics name the rule, layer, location, severity, context, and completion state."
---

# Why Validation Results Must Identify Their Sources

A validation result is actionable only when the author can understand what asserted it. “Invalid document” turns governance into a support request.

## Layers answer different questions

XML, grammar, Schematron, DITA relationships, and tenant policy should remain distinguishable.

## Location is not enough

A diagnostic should identify rule source, severity, message, content position, and relevant map or profile context.

## Incomplete is not valid

Timeouts and unavailable services must remain explicit rather than inheriting a prior green state.

## Shared diagnostics align clients

ForgeDITA returns structured results so Oxygen, web UI, automation, and audit evidence can represent the same decision.

## Why this is a product rule

ForgeDITA treats this behavior as an architectural constraint because later process cannot reliably repair an ambiguous foundation. The rule applies to the API, web interface, Oxygen integration, background workers, import and export, and conformance evidence. A convenient exception in one client is still a platform inconsistency.

## How the beta boundary applies

The current beta implements substantial parts of this model, but implementation does not turn the entire architectural target into a claim. Public status and conformance material identify partial and unsupported areas. Evaluation should use those boundaries directly and should promote a capability only when executable evidence covers the required context and failure cases.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
