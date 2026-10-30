# SkyeAtlas — Nebius × NVIDIA hackathon

Current application source is preserved in `SkyeAtlas_Source.py`, a self-extracting source distribution containing the complete unchanged Base44 export. This format avoids browser file-upload limitations. Clone/download this repository, inspect the short extractor, then run `python3 SkyeAtlas_Source.py` in an empty working directory. It verifies SHA-256 and extracts all 174 exported files into `skyeatlas/`, including frontend routes/components, server functions, entity schemas, package manifest and lockfile. Python 3.9+ is required for extraction. The extractor was tested: every extracted file matched the original export byte for byte.

Original export SHA-256: `18995a3491f80f9c65f50584c450c830bbde22697a976a3d4a9924b054cfab2f`. Read the extracted README.md and HANDOFF.md for architecture. The exported documentation predates live inference; the verification status in this root README supersedes its stale statements about no configured key/no calls/unpublished status.

Setup: Node 20+, install the official Base44 CLI, then inside the extracted folder run `npm ci`, `base44 login`, `base44 link`, `base44 dev`. Set NEBIUS_API_KEY in the linked app dashboard Secrets. Run `npm run build` and use `base44 deploy` to publish. This export requires the Base44 runtime; it is not a standalone backend.

Live app: https://skye-atlas-flow.base44.app (sign-in required). Sign in, load the fictional DEMO scenario, inspect Resume, Approvals, History, and Settings / AI. Each account has its own workspace. Set your own server-side NEBIUS_API_KEY to test inference; no key is included.

SkyeAtlas adds persistent checkpoints, source authority/version/conflict records, traffic-light autonomy, payload/version-bound approvals and before/after action receipts. NVIDIA Nemotron runs through Nebius Token Factory's OpenAI-compatible API, in src/lib/nebius.server.js. Tested model IDs: nvidia/NVIDIA-Nemotron-3-Nano-30B-A3B and nvidia/Nemotron-3_5-Lightning. No fine-tuning or dedicated GPUs. Serverless catalog and chat access avoided provisioning infrastructure.

Verified Oct 30: fictional task approval changed Blocked to Doing and produced a receipt; basic live Nemotron Lightning JSON response parsed successfully. Two complex model prompts failed the output contract. No successful evidence-grounded reasoning benchmark is claimed.

Known limits: Base44 runtime/auth/storage dependency; non-atomic action/receipt writes; concurrency and full import roundtrip unverified; dependency security findings remain unresolved. This is a hackathon prototype, not production-ready. Receipts are not immutable.

Historical July MemoryOS Lite foundation remains in the root files and git history. It is a separate deterministic proof, not the current app. The current React/server/entity implementation was developed afterward for this hackathon; preserve that distinction.

License: MIT for this project's original code; third-party packages retain their own licenses.


Demo video: https://youtu.be/O9Zsdyz4Dkw (110-second captioned walkthrough of actual authenticated screenshots, fictional records).

Gallery-only late submission: organizer granted delivery until October 31, 2026, 10 AM PT. Not eligible for judging or prizes. Source publication was completed after the competitive cutoff under this gallery-only continuation. No claim of on-time competitive submission.

Clean-workspace setup/import remains unverified; commands above are the exported project documentation, not a claim of independently reproduced deployment. Original July README is preserved in git history at commit 176d3cee6db881c3ae7b3bea286fe7b3d3951470.
