# Canonical release notes

Create exactly one Markdown entry per platform and marketing version:

```text
releases/ios/{version}.md
releases/macos/{version}.md
```

The YAML front matter is machine-validated; the Markdown body is the only authored user-facing prose. Keep entries in `draft` while editing and use `MimirRelease validate` before changing an entry to `published`.

`release_date` accepts either an exact `YYYY-MM-DD` date for new releases or a reader-friendly month and year (`June 2023`) when historical source material does not establish a publication day.

The website generator derives the public HTML pages, immutable hosted in-app Markdown, and `app/release-notes/manifest.json`. App Store Connect and TestFlight text is rendered from the same entry. Do not edit generated output or add a parallel `whats-new/` source tree.

Legacy `Mimir-*.md`, versioned TestFlight files, and the macOS plist remain available during migration. They are compatibility inputs only and must not be used for new releases.
