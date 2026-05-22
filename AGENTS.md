# AGENTS.md

## Commands
- `flutter run` — launch app on connected device/emulator
- `flutter test` — run all tests (no single-test shortcut; use `flutter test test/widget_test.dart`)
- `flutter analyze` — static analysis (lints from `analysis_options.yaml`, includes `package:flutter_lints`)
- No custom CI, task runner, or codegen scripts exist

## Structure
- Entrypoint: `lib/main.dart` (`void main()` → `runApp(MyApp)`)
- All source lives under `lib/` (currently flat, expand into subdirectories as needed)
- Tests live under `test/`, one file per feature/screen
- Standard Flutter platform directories: `android/`, `ios/`, `web/`, `linux/`, `macos/`, `windows/`

## Conventions
- Dart SDK: `>=3.4.3 <4.0.0`
- Material 3 enabled (`useMaterial3: true` in theme)
- No state management package added yet; default is `StatefulWidget` + `setState`
- No assets directory configured; add under `pubspec.yaml` `flutter: assets:` when needed
- Use Material icons (`uses-material-design: true`)

## Caveats
- No CI/CD workflows configured
- No code generation (freezed, json_serializable, etc.) — all manual Dart
