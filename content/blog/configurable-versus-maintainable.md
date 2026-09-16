---
title: "The Difference Between Configurable and Maintainable"
slug: "configurable-versus-maintainable"
category: "Architecture"
status: "draft"
description: "Why a platform can support extensive customization yet remain difficult to understand, test, upgrade, and remove."
---

# The Difference Between Configurable and Maintainable

Configurability answers whether a behavior can be changed. Maintainability asks whether the change remains understandable, testable, portable, and reversible after the original implementer is gone.

## Configuration can still be opaque

A graphical rule builder may hide dependencies as effectively as custom code if it lacks versioning and diffable representation.

## Every extension needs a lifecycle

Ownership, scope, validation, promotion, compatibility, deprecation, and rollback should be explicit.

## Scope prevents semantic drift

Platform, tenant, and workspace changes have different consequences. The system should not let a local convenience redefine global meaning silently.

## Removal is the final test

A maintainable extension can be identified, tested, upgraded, and retired. ForgeDITA favors declared packages over private platform modifications.

## The architecture test

Ask where the behavior is declared, how it is versioned, which services consume it, and what evidence shows that those services agree. If the answer changes depending on whether the user is in the editor, web interface, publishing server, or migration utility, the platform has several private architectures rather than one coherent contract.

## Design for change

A maintainable design makes dependencies visible before modification and preserves compatibility boundaries while components evolve. That requires stable APIs, explicit scopes, versioned packages, and negative tests. The objective is not architectural purity. It is the practical ability to update one part of the system without rediscovering every assumption surrounding it.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
