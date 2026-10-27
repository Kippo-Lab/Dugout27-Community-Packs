# The Dugout '27 - Community Data Packs

This public repository is the official Kippo Lab distribution point for approved community data packs for The Dugout '27.

## Creator flow

1. Build a .dugoutpack using the Dugout Pack Builder.
2. Upload that exact file as a public GitHub Release asset in your own repository.
3. Submit the direct GitHub Release asset URL through the Dugout Creator Portal.
4. GitHub Actions independently downloads the asset, verifies its SHA-256 and runs the Dugout validator.
5. Kippo Lab can approve only after server validation passes.
6. After approval, GitHub Actions downloads the same asset again, rechecks the SHA-256, validates it again, then publishes an immutable Kippo Lab GitHub Release.
7. catalog.json is updated automatically for the game.

Creators never receive write access to this repository.

## Files

- catalog.json - public catalogue used by the game.
- validation-results.json - server-side validation results for creator submissions.
- publication-results.json - publication results for approved submissions.
- .github/workflows/publish-approved-pack.yml - scheduled/manual validator and publisher.

The workflow fetches the current validator, publisher script and Firebase Web config from the deployed Kippo Lab Data Pack portal. Repository variable PORTAL_BASE_URL must point to that Firebase Hosting base URL.

## Content rules

Community packs may contain real player names and independently sourced factual/numeric football data where lawfully sourced.

Do not submit:
- player photos, face images, signatures, voices or other likeness media;
- copyrighted or trademarked logos/artwork unless the creator has the necessary rights;
- copied proprietary commercial-game ratings or substantial copied commercial databases;
- executable payloads, malicious files or unsafe archive paths.

Kippo Lab may reject, unpublish or remove a pack that fails technical, moderation, legal or safety review.

## Official database

The built-in Official Dugout Database remains fictional, unchanged and the default. Community Data Packs are optional and affect new careers only.
