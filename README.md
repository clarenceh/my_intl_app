# my_intl_app

A Flutter project to demonstrate how to perform localization.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## i18n

### Generate arb files from localization dart file

    flutter pub run intl_translation:extract_to_arb --output-dir=lib/l10n lib/localization/localizations.dart

### Generate message_xx.dart files from arb files and localzation dart file

    flutter pub run intl_translation:generate_from_arb \
        --output-dir=lib/l10n --no-use-deferred-loading \
        lib/localization/localizations.dart lib/l10n/intl_*.arb
