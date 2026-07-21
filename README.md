# Skye Cove - MemoryOS Lite

**The conversation is temporary. The user's context is portable.**

Skye Cove demonstrates a governed continuity workflow: a clean AI session retrieves the minimum current project state from a user-controlled context vault, honors authority and privacy rules, distinguishes current from superseded information, preserves unresolved conflicts, and reports exactly what it used and skipped.

## Run locally

No install, account, API key, or build step is required.

1. Download this repository.
2. Open `index.html` in Chrome, Edge, Firefox, or Safari.
3. Select **Run continuity inspection**.
4. Verify the receipt says `CONTINUITY RESTORED: PASS`.

If double-clicking does not open the page, right-click `index.html`, choose **Open with**, and select a browser.

## What is demonstrated

- A synthetic Chaz Meridian context vault, never Michael's private records.
- Source authority ranking and current-state selection.
- Superseded, restricted, unresolved, and irrelevant-source handling.
- Targeted loading and an inspectable continuity receipt.
- A compact handshake for the live connected-Drive test.

## What works now vs. what is represented

The local inspector is deterministic and fully runnable. It transparently visualizes expected governance decisions from the included synthetic dataset. The separate live ChatGPT demonstration uses a connected Google Drive and the handshake in `HANDSHAKE.md` to show assisted retrieval from a clean conversation.

This prototype does **not** claim to be an AI model, a Drive connector, automatic semantic retrieval, automatic hashing, or a production security boundary. Google Drive retrieval is a platform capability. The submission's original contribution is the portable vault structure, governance protocol, targeted handshake, provenance rules, and continuity receipt.

## Origin and provenance

This minimum build is refined from `Skye Cove Build workflow origin- RAW CHAT`, an origin/rationale conversation. The source proposed a broader system including persistent manifests, hashes, delta loading, usage preflight, and usage ledgers. This submission deliberately narrows that vision to the smallest honest proof that can run locally and be demonstrated in a clean chat.

## Repository files

- `index.html`: local Continuity Inspector.
- `vault.json`: human-readable synthetic test data.
- `HANDSHAKE.md`: live clean-session command and pass criteria.
- `DEMO_SCRIPT.md`: short recording plan.
- `SUBMISSION_COPY.md`: copy-ready project description.

## Built with Codex

Codex was used to inspect the raw workflow source, reduce scope, generate the complete prototype and documentation, and verify that the deliverable is internally consistent. No private MemoryOS records were used in the prototype.

## Future work

Portable local/Drive vault templates, content hashes and true delta comparison, automated provenance capture, user-selectable Lite/task/full refresh depth, a context-usage ledger, and platform-independent adapters.
