# Ultrahuman Ukrainian Localization

[Українською](README.uk.md)

Independent volunteer Ukrainian localization materials for the Ultrahuman Android app.

This repository is intended to make the contribution public, transparent, easy to inspect, and easy for Ultrahuman engineers to integrate if they choose to add Ukrainian language support in a future release.

## What Is Included

- Android Ukrainian resources for `res/values-uk/`
- Ukrainian Compose resource file for `com.ultrahuman.algo.resources`
- Target-only CSV and JSON formats for easier review/import
- Ukrainian and English integration guides
- Ukrainian and English content-localization proposal for articles/recommendations
- QA summary proving current resource coverage and automated language checks

## What Is Not Included

- No APK files
- No extracted proprietary binaries
- No work logs or debugging artifacts
- No full English source-string workbook in the public repository

The public formats intentionally avoid republishing the app's full English resource text. Resource keys and Ukrainian target text are included so the official Ultrahuman team can map these materials to their source project.

## Primary Integration Files

```text
localization/android/res/values-uk/strings.xml
localization/android/res/values-uk/arrays.xml
localization/android/res/values-uk/plurals.xml
localization/android/res/xml/locales_config.xml
localization/composeResources/com.ultrahuman.algo.resources/values-uk/strings.commonMain.cvr
```

## Documentation

- [Integration Guide](docs/en/integration-guide.md)
- [Content Localization Proposal](docs/en/content-localization.md)
- [QA Summary](docs/en/qa-summary.md)
- [Volunteer Outreach Text](docs/en/outreach.md)
- [Ukrainian documentation](docs/uk/README.md)

## Coverage

- 3,597 Android string resources
- 4 visible Android arrays / 74 array items
- 10 Android plural resources / 40 Ukrainian plural forms
- 304 Compose resource strings
- 4,015 rows checked by Ukrainian quality audit: 0 errors, 0 warnings

## Status

This is not an official Ultrahuman repository. It is a volunteer contribution prepared by a Ukrainian-speaking Ultrahuman user for official review and possible integration.
