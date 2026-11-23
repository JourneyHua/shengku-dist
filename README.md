# Shengku update feed

This public repository only carries the binary update feed for the private source repository
[JourneyHua/music-library](https://github.com/JourneyHua/music-library).

- `latest.json` is written by the release workflow of the source repository and always describes the
  most recent formally published version.
- Each formal tag has a release here holding exactly two assets: `Shengku-<version>-win-x64.zip` and
  its `.sha256` sidecar.
- The application reads `latest.json` anonymously and trusts only `version` and `sha256`.
- Do not upload assets or edit `latest.json` by hand; the next release would reject the mismatch.
