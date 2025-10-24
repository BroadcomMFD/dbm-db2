# Change Log

This document lists changes made to the DBM-Db2 extension.

The format of this changelog is based on [Keep a Changelog] and adheres to [Semantic Versioning].

## [Unreleased]

## 1.0.0 - 2025-10-23

### Added

- Profile auto-update upon team configuration save when Zowe Explorer is installed alongside the extension.
- Artifacts comparison between two files in the history view.
- `Analyze DDL` command lists Db2 objects in a DDL file.
  - Supports navigation and selection in a file.
  - Refreshed upon file save.
- `Deploy DDL` displays impact details and waits for confirmation before committing changes.
- Navigation to a profile in the team configuration upon selecting for editing.

### Changed

- `Verify DDL` command renamed to `Check DDL Execution`.
- History record click opens contextual information for the selected file, showing the choices, profiles, and timestamp
  at the time of operation start.
- History DDL file click opens DDL analysis.
- History files are now read-only with an easy way to enable editing.
- History file changes are automatically saved along with the original (single copy).
- `Deploy DDL` confirmation popup changed to a webview that allows reviewing and changing input.

## 0.3.0 - 2025-04-28

### Added

- `Check DDL Syntax` operation.
- `Verify DDL Dependencies` operation.
- `Copy Objects` operation.
- `Save As` command for history files.
- Unsaved document processing.
- Partial document processing.
- DDL Analysis after the `Generate DDL` operation.

### Changes

- Status bar reflects Db2 subsystem upon which operation is performed.
- History files opened as copies.

### Fixed

- Virus detection issue.

## 0.2.3 - 2025-03-05

### Fixed

- Updated dependencies to resolve false-positive virus discovery.

## 0.2.2 - 2024-10-15

### Removed

- `Zowe Explorer` extension dependency.

## 0.2.1 - 2024-10-08

### Added

- Zowe Explorer V3 support.

## 0.2.0 - 2024-09-30

### Added

- Execution profiles selection.
- `Deploy DDL` operation.
- `Db2 Management History` view.
- Status Bar items for the selected Db2 and the selected execution profile.

## 0.0.1 - 2024-05-28

Initial release.

### Added

- `Db2 Schema Management` view.
- `Generate DDL` operation.

[Keep a Changelog]: https://keepachangelog.com/en/1.1.0/
[Semantic Versioning]: https://semver.org/spec/v2.0.0.html
