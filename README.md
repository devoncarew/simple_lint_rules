[![Dart CI](https://github.com/devoncarew/simple_lint_rules/actions/workflows/build.yaml/badge.svg)](https://github.com/devoncarew/simple_lint_rules/actions/workflows/build.yaml)
[![pub package](https://img.shields.io/pub/v/simple_lint_rules.svg)](https://pub.dev/packages/simple_lint_rules)

## What is this?

A simple lint rule set and analysis options configuration. This rule set is
based on `package:lints/recommended.yaml`.

## Using the Lints

To use the lints, add a dependency in your `pubspec.yaml` file:

```yaml
dev_dependencies:
  simple_lint_rules: ^2.0.0
```

then, add an `analysis_options.yaml` file to your project:

```yaml
include: package:simple_lint_rules/strict.yaml
```

or:

```yaml
include: package:simple_lint_rules/strict_plus.yaml
```

## Contributions, PRs, and publishing

When contributing to this repo:

- if the version in the changelog is a stable semver version (`x.y.z`), the
  latest changes there have been published to pub. Please add a new changelog
  section for your change, rev the service portion of the version and append
  `-dev`, and update pubspec.yaml to agree with the new version
- if the changelog version ends in `-dev`, the latest changes are unpublished;
  please add a new changelog entry for your change in the most recent section
- for PRs, the `Publish` bot will perform basic validation of the info in the
  pubspec.yaml and CHANGELOG.md files
- when the PR is merged into the main branch, if the change is for an
  unpublished stable version, a repo maintainer will tag that commit with the
  pubspec version (e.g., `v1.2.3`); that tag event will trigger the `Publish`
  bot to publish a new version of the package to pub.dev
