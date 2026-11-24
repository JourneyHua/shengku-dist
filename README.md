# Shengku binary distribution

This public repository hosts official Windows x64 application packages and the anonymous in-app update feed.

- Each formal release contains the application ZIP and its SHA256 sidecar.
- The release workflow maintains latest.json, which points to the newest formally published version.
- The app reads the feed anonymously and validates package compatibility, size, and SHA256 before installation.
- Do not upload release assets or edit latest.json manually.