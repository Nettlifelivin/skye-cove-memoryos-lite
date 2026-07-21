# Submission copy

## Name

Skye Cove - MemoryOS Lite

## One-line pitch

A user-owned context vault and compact handshake that restore governed project continuity in a clean AI session without reloading everything.

## Problem

People repeatedly spend time, tokens, privacy, and cognitive effort reconstructing context that they have already organized. Conversation history is not a transparent governance system: users need to know which source controlled, what was superseded, what stayed private, and what remains uncertain.

## Solution

Skye Cove treats durable context as a portable, user-controlled layer. A clean session receives one targeted handshake, retrieves the minimum relevant sources, applies authority and privacy rules, and returns both useful current state and a continuity receipt. A no-install local inspector makes the same decisions visible with synthetic data.

## How it works

The included manifest assigns each source an identity, authority rank, privacy class, status, and modification date. The prototype selects the governing baseline, skips superseded and irrelevant material, blocks restricted content, preserves unresolved claims, and shows its work. `HANDSHAKE.md` provides the corresponding clean-session Drive test.

## Impact

The workflow reduces repeated explanation, limits unnecessary disclosure, and makes continuity portable across chats, accounts, projects, and eventually AI platforms. It is designed to become a starter vault that nontechnical people can fill gradually and keep under their control.

## Built during Build Week

Codex helped convert a broad pre-existing MemoryOS architecture into this new, bounded demonstration: source extraction, scope reduction, synthetic dataset design, complete local prototype, test criteria, documentation, and demo packaging.

## Limitations

The local inspector is deterministic. It does not perform AI retrieval or connect to Drive. The live demo relies on ChatGPT's connected-Drive capability and manual orchestration. Automated hashes, delta detection, usage accounting, and cross-platform adapters are future work.
