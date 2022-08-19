[![Dart CI](https://github.com/devoncarew/simple_lint_rules/actions/workflows/build.yaml/badge.svg)](https://github.com/devoncarew/simple_lint_rules/actions/workflows/build.yaml)
[![pub package](https://img.shields.io/pub/v/simple_lint_rules.svg)](https://pub.dev/packages/simple_lint_rules)

## What is this?

A simple lint rule set and analysis options configuration for Dart's analysis
server. This rule set is based on `package:lints/recommended.yaml`.

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
