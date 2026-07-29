# Change Log

This document lists changes made to the DBM-Db2 extension.

The format of this changelog is based on [Keep a Changelog] and adheres to [Semantic Versioning].

## [Unreleased]

## [1.0.9][marketplace] - 2026-07-15

This release includes minor security improvements. An update is recommended.

## [1.0.8][marketplace] - 2026-07-03

This release includes minor security improvements. An update is recommended.

### Changed

- Deploy DDL impact report table columns now have a fixed width.

### Fixed

- The Deploy DDL webview spinner now stops when a failure occurs.
- Deploy DDL now supports the old DBM DS template that did not return the customized DDL.

## [1.0.7][marketplace] - 2026-03-16

### Added

- Extended trace logging to include Zowe Imperative log records.

## [1.0.6][marketplace] - 2026-03-12

### Added

- Extended logging in the `DBM-Db2` section of the VS Code `Output` panel.

## [1.0.5][marketplace] - 2026-02-27

This release includes minor security improvements. An update is recommended.

### Changed

- The error file now shows the most relevant information first.
- The error file now includes additional contextual information.
- An error file is now created for connection errors.

## [1.0.4][marketplace] - 2026-01-16

This release includes minor security improvements. An update is recommended.

## [1.0.3][marketplace] - 2025-12-17

This release includes minor security improvements. Update is recommended.

Third party component React upgraded from 19.0.1 to 19.2.3. Although Code4z extension for Db2 for z/OS schema
management include a version of React impacted by CVE-2025-55184, based on the information disclosed by React and
investigation conducted by our teams at this time, Code4z extension for Db2 for z/OS schema management is not affected
by CVE-2025-55182 because it does not use React Server Components. To prevent future possible exposure to this
vulnerability, out of abundance of caution, we are providing this maintenance update to upgrade React.

### Fixed

- `Update Credentials` is now triggered correctly.
- Db2 subsystems with same-named data sharing groups are now displayed correctly.

## [1.0.2][marketplace] - 2025-12-11

This release includes minor security improvements. Update is recommended.

Third party component React upgraded from 19.0.0 to 19.0.1. Although Code4z extension for Db2 for z/OS schema
management include a version of React impacted by CVE-2025-55182, based on the information disclosed by React and
investigation conducted by our teams at this time, Code4z extension for Db2 for z/OS schema management is not affected
by CVE-2025-55182 because it does not use React Server Components. To prevent future possible exposure to this
vulnerability, out of abundance of caution, we are providing this maintenance update to upgrade React.

## [1.0.1][marketplace] - 2025-12-03

This release includes minor security improvements. Update is recommended.

### Changed

- The `terminationCharacter` default value changed to `#` when a new profile is created.

### Fixed

- Non-default termination characters are now supported in the `Analyze DDL` command.

## [1.0.0][marketplace] - 2025-10-23

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
[marketplace]: https://marketplace.visualstudio.com/items?itemName=broadcomMFD.dbm-db2
