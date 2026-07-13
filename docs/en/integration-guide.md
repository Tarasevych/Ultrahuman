# Integration Guide

[Українською](../uk/integration-guide.md)

## 1. Add Android Ukrainian Resources

Add the Ukrainian resources to the Android module that owns the existing default resources:

```text
app/src/main/res/values-uk/strings.xml
app/src/main/res/values-uk/arrays.xml
app/src/main/res/values-uk/plurals.xml
```

Repository files:

```text
localization/android/res/values-uk/strings.xml
localization/android/res/values-uk/arrays.xml
localization/android/res/values-uk/plurals.xml
```

## 2. Register Ukrainian Locale

The inspected app already declares:

```xml
android:localeConfig="@xml/locales_config"
```

Add Ukrainian:

```xml
<locale android:name="uk" />
```

An example updated file is included:

```text
localization/android/res/xml/locales_config.xml
```

## 3. App Bundle / Language Split

The installed Android package already uses language splits, for example Dutch via `split_config.nl.apk`. After `values-uk` is present and `uk` is included in locale config/build settings, the App Bundle pipeline should be able to produce a Ukrainian language split.

## 4. Add Compose Resources

The app also contains Compose resources under `composeResources/com.ultrahuman.algo.resources`. Add:

```text
localization/composeResources/com.ultrahuman.algo.resources/values-uk/strings.commonMain.cvr
```

This mirrors existing locale folders such as `values-nl`, `values-pl`, and others.

## 5. Import Alternatives

If the team uses a localization platform, target-only files are available:

```text
formats/csv/*.csv
formats/json/*.json
```

The public repository intentionally omits full English source-string workbooks. Ultrahuman can map by resource key inside the official source project.

## 6. Required Final QA

Before release, Ultrahuman should verify Ukrainian in a signed internal build:

- text fitting in buttons, cards, dialogs, charts, Ring setup, and notifications;
- server-driven/runtime strings not present in static resources;
- Google Play language split delivery;
- tone alignment with Ultrahuman product voice.

The volunteer contributor can continue QA after Ukrainian is enabled in a test build or production rollout.
