---
title: "Why the Editor Is a Client, Not the System"
slug: "editor-client-not-system"
category: "ForgeDITA"
status: "draft"
description: "How a server-authoritative authoring contract preserves editor quality without creating editor lock-in."
---

# Why the Editor Is a Client, Not the System

Oxygen provides a professional XML authoring experience. ForgeDITA treats that strength as a client capability, not as permission to hide repository truth or business rules inside the editor.

## The server owns durable state

Locks, revisions, permissions, workflow, graph state, validation results, and publishing jobs remain authoritative outside the client.

## Clients share one contract

Oxygen, a web interface, automation, and future editors use the same documented APIs.

## Convenience may vary

A rich editor can offer better navigation and markers while preserving identical server semantics.

## Thin does not mean weak

The integration can be sophisticated without possessing private endpoints or interpretations unavailable to other authorized tools.

## Why this is a product rule

ForgeDITA treats this behavior as an architectural constraint because later process cannot reliably repair an ambiguous foundation. The rule applies to the API, web interface, Oxygen integration, background workers, import and export, and conformance evidence. A convenient exception in one client is still a platform inconsistency.

## How the beta boundary applies

The current beta implements substantial parts of this model, but implementation does not turn the entire architectural target into a claim. Public status and conformance material identify partial and unsupported areas. Evaluation should use those boundaries directly and should promote a capability only when executable evidence covers the required context and failure cases.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
