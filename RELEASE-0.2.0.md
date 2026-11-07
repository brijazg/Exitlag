# Release 0.2.0 — Documentation maintenance update

**Status:** maintenance update prepared for review. This is a documentation-site version, not an ExitLag VPN application release.

## Changes

- Bumped the documentation package version from 0.1.0 to 0.2.0.
- Declared Node.js 18.14+ as the supported runtime baseline.
- Replaced the outdated GitHub Actions checkout/setup-node v2 steps with v4.
- Expanded CI to run on pushes, pull requests targeting `main`, and manual dispatch.
- Added read-only workflow permissions, concurrency cancellation, and a job timeout.
- Made dependency installation reproducible with `yarn install --frozen-lockfile`.
- Updated the README with accurate setup, build, translation, contribution, and deployment guidance.
- Clarified that this repository contains Manta Network documentation and is not the ExitLag VPN application.

## Validation

The GitHub Actions workflow is configured to install the locked dependencies and run `yarn build`. A release should only be considered verified after that workflow completes successfully.

## Not included

- No broad dependency upgrades were performed; the existing dependency tree and lockfile were retained to avoid an unreviewed breaking migration.
- No production deployment was triggered.
- No claim is made that every documentation page or external link has been manually verified.
