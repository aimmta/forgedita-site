---
title: "Publishing Drift Is an Architecture Problem"
slug: "publishing-drift-architecture-problem"
category: "Publishing"
status: "published"
published: "2026-08-25"
description: "Why DITA publishing environments drift, why procedural discipline cannot fully contain the problem, and how versioned toolchains restore control."
---

# Publishing Drift Is an Architecture Problem

Publishing drift rarely announces itself. A plugin changes, a catalog is patched, a runtime is upgraded, or a transform is corrected directly on a server. Each change may be reasonable. The problem is that the publication no longer has a durable relationship to a fully identified processing environment.

## Drift begins with ambient configuration

Many publishing systems treat the active DITA-OT installation as infrastructure rather than as a release input. That makes the build depend on whatever happens to be installed when the job runs. The content may be versioned carefully while the code interpreting it remains mutable. A successful build proves only that the current environment produced an output, not that the approved environment did.

## Process cannot reconstruct missing state

Teams respond with checklists, release notes, server snapshots, and knowledgeable administrators. Those practices reduce risk, but they cannot prove a state the system never captured. If the exact plugins, catalogs, parameters, validation assets, and runtime identity are missing, the release record contains an assumption rather than evidence.

## Make the toolchain an input

A reproducible publishing model identifies an immutable content baseline, an immutable toolchain bundle, and a named publish profile. The resulting manifest records the artifacts and their fingerprints. A rebuild can then compare identified inputs and outputs instead of asking someone to remember which server was considered correct at the time.

## The practical evaluation question

Ask a CCMS vendor to rebuild a release from a year ago while the current publishing environment remains unchanged. Then ask for the exact toolchain manifest used by both builds. The answer reveals whether reproducibility is an architectural property or a process aspiration. ForgeDITA treats publishing configuration as governed release data because output trust depends on it.

## The ForgeDITA position

ForgeDITA is being built around explicit contracts, native content, contextual DITA semantics, and evidence that can be inspected. Current beta limitations are published openly so evaluators can distinguish implemented behavior from the complete architectural target.
