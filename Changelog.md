# Changelog

The notable changes of n4u_mlomerger, by version. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and the versions follow [Semantic Versioning](https://semver.org/).

## [Unreleased]

## [1.0.0] - 2026-11-20

This is the first official version !!

### Changed

- **The merge deploys only the stream files the game build loads.** DLCs ship many vanilla map files again under
  prefixes of their own (`hei_`, `apa_`, ...), and the game loads one of each. The merge now deploys only the one
  `sv_enforceGameBuild` loads and carries the resources' changes to the others over to it, so that their items are no
  longer placed twice. The build is set by `Config.mlomerger.enforcedGameBuild` (`sv_enforceGameBuild` by default).
  The item lists show each item as the loaded file has it; the details mark the other files as past or future ones.
- Smaller changes: the stream file search can be resized against the editors' buttons; nothing of the editor runs while
  the in-game menu is closed; the entity list shows the high-detail LOD levels by default; the messages asking for a
  merge point to `mlomerger apply`; the markers of vanilla items an overwrite removes are crossed out in red; the
  overwrites are written minified.

### Added

- **LOD relations**: the entity details show the entity's LOD parent and children, which can be opened, selected,
  removed and turned on or off wherever they are.
- **Stream file search by name**: the top page finds the stream files by name as it is typed, besides at a position.
- **A page for one ymap**: every item of a ymap in one list, in the file's order, opened with → beside the file in the
  top page's search.
- **Resources page**: the resources mlo_merger recognizes, with how much each changes vanilla and what is left out of
  the merge.
- **Vanilla page**: reserved on the top page; not implemented yet.
- Smaller additions: an overwrite warning about a ymap leads to the page of its items, a warned overwrite can be removed
  from the warning, and a warning saved as fixed tells so until the next Save & apply.

## [0.1.0] - 2026-11-12

### Added

- First release: the merge of MLO and map resources against vanilla on server start, with connections held until the
  merged resource is deployed, and the in-game menu (`/mlomerger`).
