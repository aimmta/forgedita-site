---
title: "What a Public DITA Conformance Statement Should Contain"
slug: "public-dita-conformance-statement"
category: "Conformance"
status: "published"
published: "2026-08-27"
description: "A practical model for specific, testable, versioned DITA conformance claims that include limitations instead of hiding them."
---

# What a Public DITA Conformance Statement Should Contain

The phrase “DITA compliant” sounds precise, but it often tells an evaluator very little. DITA contains multiple document types, processing features, reuse mechanisms, filtering rules, specialization behavior, and contextual resolution requirements. A useful claim must say which of those behaviors are supported and what evidence supports the statement.

## Name the specification and boundary

A conformance statement should identify the DITA version, supported feature families, processing assumptions, and explicit exclusions. Storage of a DITA file is not the same as correct processing of its semantics. The statement should separate preservation, authoring operations, validation, resolution, publishing, and interoperability.

## Connect claims to executable evidence

Every claimed behavior should have a stable identifier and a repeatable fixture. Evidence should record the implementation version, inputs, expected result, actual result, outcome, and relevant hashes. Negative cases matter as much as successful cases because broken catalogs, missing keys, circular reuse, and unauthorized operations reveal whether the system fails honestly.

## Publish partial and unsupported areas

A credible statement includes what is partial and what is not claimed. That protects buyers from broad language and gives engineering teams a visible promotion path. A feature should move into the claimed set only when the product, test fixtures, and published statement agree.

## Treat the statement as a generated contract

Hand-maintained matrices eventually drift from implementation. The stronger model generates the public statement from versioned evidence and removes a claim when its tests fail. ForgeDITA uses this bounded approach because an honest limitation is operationally useful, while an unqualified compliance slogan is not.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
