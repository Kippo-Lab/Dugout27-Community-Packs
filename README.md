# The Dugout '27 — Community Data Packs

This repository is the official Kippo Lab distribution point for **approved** community data packs for The Dugout '27.

## Important

- The built-in **Official Dugout Database** remains fictional, unchanged, and the default.
- Community Data Packs are optional and apply only to **new careers**.
- Existing careers keep the world/version they were created with.
- Only packs that pass Dugout validation and moderation are published here.

## Creator flow

1. Build a `.dugoutpack` using the Dugout Pack Builder.
2. Upload the pack as a **GitHub Release asset in your own GitHub repository**.
3. Submit that GitHub Release download link through the Dugout creator submission page.
4. Kippo Lab reviews and validates the pack.
5. If approved, the exact approved file is copied to a Kippo Lab release in this repository.
6. The in-game catalogue points players to the Kippo Lab-hosted approved copy.

Creators do **not** receive write access to this repository.

## Data/content rules

Community packs may contain real player names and independently sourced factual/numeric football data where lawfully sourced.

Do not submit:
- player photos, faces, likeness images, signatures, or voices;
- copyrighted or trademarked logos/artwork unless you have the necessary rights;
- copied proprietary commercial-game ratings or substantial copied commercial databases;
- malicious files, executable payloads, or unsafe archive paths.

Kippo Lab may reject, unpublish, or remove a pack that fails technical, moderation, legal, or safety review.

## File format

Approved files use the `.dugoutpack` extension. A pack is a ZIP-compatible archive and must pass the Dugout validator before publication.

## Publishing

The workflow in `.github/workflows/publish-approved-pack.yml` is intentionally manual. It downloads an already-approved creator-hosted GitHub Release asset, verifies its SHA-256, and then publishes a new immutable Kippo Lab GitHub Release.
