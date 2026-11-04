# Admiral Game Afterglow source snapshot

Source: https://github.com/well0nez/afterglow-web
Commit: `acf25a831725f0d44fcb64725d4ce35acbba8f9d` (3 November 2026).
Production route: `https://admiralgame.my.id/ps4/afterglow/`.

This directory preserves the upstream browser exploit, payloads, patch sets,
README, technical notes, and license files. Text files use LF line endings so
their bytes match the live upstream site. Binary files are byte-for-byte copies.
The Admiral Pages build verifies all 15 hashed assets in `cache.appcache` and
publishes a manifest with each hash comment on its own line. Its Pages Worker
serves the listed `index.html` and `jb.html` URLs directly, since Pages would
otherwise redirect them and prevent AppCache installation. The exploit code
and payload bytes are not changed by those hosting steps.

Binary SHA-256:

- `hen.bin` — `364e5f6fd59e8a7afc207c70e27b840699f8173f3ae0241b63bc6dec6b394bfe`
- `goldhen.bin` — `39452f5e1c305ac9efcb4745eef7958b4db8c6d85299529f08700970b009ea4d`
- `patchset-1400.bin` — `615f275b96831cc04173757db39e93f0d27b52888976af2a6444604aa8ac5dbf`
- `patchset-1352.bin` — `adfb9771904f71cd1f5a82cbded8ac46c7ffeb3df974579535cf711904ac347e`

Afterglow's own code and patch sets use AGPL-3.0-or-later. The raw13g files
retain `LICENSE-raw13g`. See upstream `README.md` and `TECHNICAL.md` for other
provenance and warnings. This snapshot is kept separate from the existing
Admiral 6.72–13.52 chain and payloads.
