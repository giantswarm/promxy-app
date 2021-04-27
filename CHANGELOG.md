# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.12.0] - 2021-04-27

### Removed

- Remove unneeded managed-by label

## [0.11.0] - 2021-04-20

### Added

- Added `Ingress` resource for root of the prometheus domain and for OAuth
  proxy to prepare for moving Promxy to `/`

## [0.10.0] - 2021-04-19

### Changed

- Updated promxy to v0.0.70

## [0.9.0] - 2021-04-09

### Added

- Add `application.giantswarm.io/team` annotation to Chart.yaml for routing
alerts.
- Add Management Cluster configmap

## [0.8.0] - 2021-02-08

### Changed

- Updated promxy to v0.0.67

## [0.7.0] - 2020-12-09

### Changed

- Updated promxy to v0.0.62

## [0.0.6] - 2020-10-08

### Added

- Added limits

## [0.0.4] - 2020-10-07

### Changed

- Increased number of replicas to 2

### Removed

- Removed limits

## [0.0.3] - 2020-10-07

### Added

- Added ingress

## [0.0.2] - 2020-10-01

### Added

- Added healthchecks and allow port configuration
- Define resource requests/limits to help with scheduling
- Set monitoring labels and annotations so the service is picked up by Giant Swarm monitoring

## [0.0.1] - 2020-09-29

### Added

- Create initial chart

[Unreleased]: https://github.com/giantswarm/promxy-app/compare/v0.12.0...HEAD
[0.12.0]: https://github.com/giantswarm/promxy-app/compare/v0.11.0...v0.12.0
[0.11.0]: https://github.com/giantswarm/promxy-app/compare/v0.10.0...v0.11.0
[0.10.0]: https://github.com/giantswarm/promxy-app/compare/v0.9.0...v0.10.0
[0.9.0]: https://github.com/giantswarm/promxy-app/compare/v0.8.0...v0.9.0
[0.8.0]: https://github.com/giantswarm/promxy-app/compare/v0.7.0...v0.8.0
[0.7.0]: https://github.com/giantswarm/promxy-app/compare/v0.0.6...v0.7.0
[0.0.6]: https://github.com/giantswarm/promxy-app/compare/v0.0.4...v0.0.6
[0.0.4]: https://github.com/giantswarm/promxy-app/compare/v0.0.3...v0.0.4
[0.0.3]: https://github.com/giantswarm/promxy-app/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/giantswarm/promxy-app/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/giantswarm/promxy-app/releases/tag/v0.0.1
