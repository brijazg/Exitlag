# Manta Network Documentation

This repository contains the Manta Network documentation website, built with [Docusaurus 2](https://docusaurus.io/). The published documentation is hosted at [docs.manta.network](https://docs.manta.network).

> **Repository note:** this repository is a fork/customized copy of the Manta Network documentation project. It is not the ExitLag VPN application or its source code.

## Current project version

**0.2.0** — see [RELEASE-0.2.0.md](RELEASE-0.2.0.md) for the maintenance update notes.

## Requirements

- Node.js 18.14 or newer (CI currently uses Node.js 18.20.8)
- Yarn Classic (1.x)
- Git

## Install dependencies

From the repository root:

```bash
corepack enable
yarn install --frozen-lockfile
```

If you intentionally change dependencies, update and commit `yarn.lock` with the same change.

## Run locally

```bash
yarn start
```

Docusaurus starts a local development server and refreshes the page as files change.

## Build and preview

```bash
yarn build
yarn serve
```

The production site is generated in the `build/` directory. The build command also checks broken links according to the configuration in `docusaurus.config.js`.

## Translations

The configured locales are English (`en`, default) and Chinese (`cn`).

Start the Chinese site locally with:

```bash
yarn start --locale cn
```

Translation content belongs under the matching Docusaurus locale directory. Do not add another locale without updating the `i18n.locales` configuration.

## Deployment

The Docusaurus deployment configuration currently targets the official Manta documentation site and repository. Do not run `yarn deploy` from a personal fork unless you are an authorized maintainer and have confirmed the deployment target and credentials.

For normal contributions, create a branch, run the production build, and open a pull request against `main`.

## Continuous integration

GitHub Actions runs the dependency installation and production build on pushes and pull requests targeting `main`. The workflow uses a pinned Node.js 18 release, Yarn's frozen lockfile mode, read-only repository permissions, and a bounded job timeout.

## Contributing

- Keep documentation links and sidebar entries in sync.
- Verify code samples and network details against current official Manta sources before changing them.
- Never commit private keys, seed phrases, access tokens, or personal credentials.
- Include the affected page and steps to reproduce when reporting a build or documentation issue.
