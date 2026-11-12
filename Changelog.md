# Changelog

The notable changes of n4u_mlomerger, by version. The format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and the versions follow [Semantic Versioning](https://semver.org/).

## [Unreleased]

## [0.1.0] - 2026-11-12

### Added

- First release: the merge of MLO and map resources against vanilla on server start, with connections held until the
  merged resource is deployed, and the in-game menu (`/mlomerger`).
- The installation check, in the server console on start (and `mlomerger setup`) and on the Setup page of the in-game
  menu, with the check for a newer release (`checkForUpdates`).
