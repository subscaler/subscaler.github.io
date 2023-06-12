# Subscaler

An opinionated suite of patterns, tools, and practices to help sublinearly scale your engineering systems.

Sublinearly scaling a repository requires thinking differently. There's often no "one size fits all" solution to how to scale. Instead there's a set of principles, and ideas that all culminate in an ecosystem and a culture of thinking which lends itself to easily growing without the confines of some overarching, and limitng tool.

## Principles

> Do one thing, and one thing well.

Every tool we own or recommend should do one thing, and do that one thing well.

> Do things fast

The tools we recommend will do one thing they do with performance and scale first thinking. We build for the use case of thousands of packages.

## Subscaler Up
Automatically enhances your monorepo with a command line tool that walks through adding tools to your new or existing
repository to help sublinearly scale.

```bash
npm i -g @subscaler/up
sup init
```

## Package Installer
Rapidly installs packages from NPM. Do one thing, and one thing well.

```bash
npm i -g @subscaler/package-installer
spm install
```

## Task Runner
We generally encourage teams to leverage the amazing work of [lage](https://github.com/microsoft/lage) for running tasks at scale.

```bash
npm i lage
lage run build test lint
```

However, we also leverage [BuildXL](https://github.com/microsoft/buildxl) in CI/CD for it's caching, and distribution story.


## Semver Managemnt
[Beachball](https://github.com/microsoft/beachball) is our recommended path to scale your repository.

```bash
npm i -g beachball
beachball change
beachball bump
```

## Version Management
For maintaining specific versions of specific packages or groups of packages, we use a tool called [@rnx-kit/depcheck](https://github.com/microsoft/rnx-kit/tree/main/packages/dep-check)

```bash
npm add --save-dev @rnx-kit/dep-check
```
