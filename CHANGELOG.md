## 2.0.0

- Upgrade to Dart `2.19.0`
- Use analyzer language modes instead of deprecated `strong-mode`

  ```yaml
  language:
    strict-casts: true
    strict-inference: true
    strict-raw-types: true
  ```

- Enable lints:
  - avoid_print
  - unnecessary_to_list_in_spreads
  - prefer_single_quotes
  - use_enums

- Disable lints:
  - avoid_returning_null_for_future
  - prefer_foreach
  - prefer_mixin

## 1.0.0

- Initial release
