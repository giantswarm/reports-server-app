# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Changed

- Prefer scheduling reports-server pods on the same node as their CNPG postgres instance, and prefer spreading reports-server replicas across nodes.
- Add Giant Swarm team labels to monitoring resources.
- Disable CNPG operator-managed `PodMonitor` in favor of a new chart-managed `PodMonitor`.

## [0.1.2] - 2026-04-16

### Changed

- Update CiliumNetworkPolicy to allow postgres cross-pod health checks.
- Enable observability platform collection for postgres and reports-server pods.

## [0.1.1] - 2026-04-10

### Added

- Add `io.giantswarm.application.audience` and `io.giantswarm.application.managed` chart annotations for Backstage visibility.
- Push to the `default` catalog.

### Changed

- Migrate chart metadata annotations to OCI-compatible format.

## [0.1.0] - 2026-01-16

### Changed

- Update to reports-server v0.1.6.

## [0.0.3] - 2025-10-23

### Added

- Add PodLogs for log collection.

## [0.0.2] - 2024-06-04

### Added

- Add Cilium Network Policies for reports-server and managed Postgres instances.
- Push to AWS app collection.

## [0.0.1] - 2024-05-17

### Added

- Initial release using [an unreleased upstream version `f97f31`](https://github.com/kyverno/reports-server/tree/f97f31a8db43d1b70a8ab903b0e11d61679ae75e).

[Unreleased]: https://github.com/giantswarm/reports-server-app/compare/v0.1.2...HEAD
[0.1.2]: https://github.com/giantswarm/reports-server-app/compare/v0.1.1...v0.1.2
[0.1.1]: https://github.com/giantswarm/reports-server-app/compare/v0.1.0...v0.1.1
[0.1.0]: https://github.com/giantswarm/reports-server-app/compare/v0.0.3...v0.1.0
[0.0.3]: https://github.com/giantswarm/reports-server-app/compare/v0.0.2...v0.0.3
[0.0.2]: https://github.com/giantswarm/reports-server-app/compare/v0.0.1...v0.0.2
[0.0.1]: https://github.com/giantswarm/reports-server-app/releases/tag/v0.0.1
