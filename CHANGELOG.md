# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed

- Ingress: Use `ImplementationSpecific`. ([#161](https://github.com/giantswarm/promxy-app/pull/161))

## [1.22.0] - 2023-10-03

### Changed

- Add condition for PSP installation in helm chart.

## [1.21.0] - 2023-09-27

### Added

- Possibility to configure used ClusterIssuer name for Ingresses.

## [1.20.0] - 2023-07-04

### Changed

- Add Service Monitor.

## [1.19.0] - 2023-06-27

### Added

- Add `push to capz-app-collection` to circleci
- Add Kyverno Policy Exceptions.

### Changed

- Upgrade Promxy to v0.0.81.

## [1.18.0] - 2023-06-15

### Removed

- Stop pushing to `openstack-app-collection`.
- Remove pull secret from chart.

## [1.17.2] - 2023-03-02

### Added

- Add additional annotations on all `ingress` objects to support DNS record creation via `external-dns`.
- Added the use of the runtime/default seccomp profile.

## [1.17.1] - 2023-01-10

### Changed

- Deploy to GCP.

## [1.17.0] - 2022-11-25

## Changed

- resources limits and request can now be defined in values

## [1.16.1] - 2022-11-08

### Changed

- Push to `capa-app-collection`, `cloud-director-app-collection`, `openstack-app-collection` and `vsphere-app-collection`.

## [1.16.0] - 2022-07-04

## Changed

- Upgrade promxy from 0.0.70 to 0.0.75 - see [promxy releases](https://github.com/jacksontj/promxy/releases)

## [1.15.0] - 2022-06-13

### Fix

- Run promxy as a non root user.

## [1.14.0] - 2022-02-16

### Changed

- Changed Ingress template to use at least `networking.k8s.io/v1beta1` or `networking.k8s.io/v1` where available.

## [1.13.1] - 2021-09-13

### Fixed

- OAuth not working by adding a separate basic auth ingress.

## [0.13.0] - 2021-06-03

### Added

- Added dual-auth for Promxy at the root of the prometheus domain as OAuth2 is
  more user-friendly and we can still preserve basic-auth for programmatic
  access by allowing access if any auth mechanism succeeds.

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

[Unreleased]: https://github.com/giantswarm/promxy-app/compare/v1.22.0...HEAD
[1.22.0]: https://github.com/giantswarm/promxy-app/compare/v1.21.0...v1.22.0
[1.21.0]: https://github.com/giantswarm/promxy-app/compare/v1.20.0...v1.21.0
[1.20.0]: https://github.com/giantswarm/promxy-app/compare/v1.19.0...v1.20.0
[1.19.0]: https://github.com/giantswarm/promxy-app/compare/v1.18.0...v1.19.0
[1.18.0]: https://github.com/giantswarm/promxy-app/compare/v1.17.2...v1.18.0
[1.17.2]: https://github.com/giantswarm/promxy-app/compare/v1.17.1...v1.17.2
[1.17.1]: https://github.com/giantswarm/promxy-app/compare/v1.17.0...v1.17.1
[1.17.0]: https://github.com/giantswarm/promxy-app/compare/v1.16.1...v1.17.0
[1.16.1]: https://github.com/giantswarm/promxy-app/compare/v1.16.0...v1.16.1
[1.16.0]: https://github.com/giantswarm/promxy-app/compare/v1.15.0...v1.16.0
[1.15.0]: https://github.com/giantswarm/promxy-app/compare/v1.14.0...v1.15.0
[1.14.0]: https://github.com/giantswarm/promxy-app/compare/v1.13.1...v1.14.0
[1.13.1]: https://github.com/giantswarm/promxy-app/compare/v0.13.0...v1.13.1
[0.13.0]: https://github.com/giantswarm/promxy-app/compare/v0.12.0...v0.13.0
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
