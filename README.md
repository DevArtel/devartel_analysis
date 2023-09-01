# devartel_analysis

## Usage

1. Add this package to **dev_dependencies**

```yaml
dev_dependencies:
  devartel_analysis:
    git:
      url: https://github.com/DevArtel/devartel_analysis.git
      ref: v3.0.0
```

2. Create an `analysis_options.yaml`

Example `analysis_options.yaml` file:

```yaml
include: package:devartel_analysis/analysis_options.yaml
```

Or imports lints only:

```yaml
# This imports only lints
include: package:devartel_analysis/lints.yaml

analyzer:
  # Provide your analyzer configuration here
```

## Enable/Disable individual rules

This package is customizable, you can change rules depending on project needs.
To do so adjust your `analysis_options.yaml`.

```yaml
include: package:devartel_analysis/analysis_options.yaml

linter:
  rules:
    # Disable individual rules
    always_put_required_named_parameters_first: false
    avoid_classes_with_only_static_members: false

    # Enable individual rules
    sort_constructors_first: true
    prefer_single_quotes: true
```

## Using with analyzer plugins

```yaml
include: package:devartel_analysis/analysis_options.yaml

analyzer:
  plugins:
    - dart_code_metrics
  exclude:
    - "lib/**/*.g.dart"
    - "lib/**/*.freezed.dart"
```
