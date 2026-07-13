# Ukrainian Content Localization Proposal

[Українською](../uk/content-localization.md)

The static language pack covers Android and Compose UI resources. Articles, recommendations, educational cards, and other reading content may be server-driven or CMS-driven, so they may not be present in APK resources.

## Recommended Behavior

When the app UI language is Ukrainian (`uk` / `uk-UA`), the app/backend should request Ukrainian content where available:

- app locale: `uk` or `uk-UA`
- CMS/backend locale: Ukrainian
- fallback: English when Ukrainian content is not yet available

## Suggested Workflow

1. Export source articles/recommendations from Ultrahuman's official CMS or localization platform.
2. Provide content as Markdown, HTML, CSV, XLIFF, JSON, Lokalise, Crowdin, Phrase, or another internal format.
3. Translate with the same glossary used for the app UI.
4. Preserve wellness/medical nuance and avoid overclaiming outcomes.
5. Import Ukrainian content back into the CMS.
6. Test that Ukrainian users receive Ukrainian content and English fallback only where needed.

## Volunteer Support

The contributor can help translate and review Ukrainian content after Ultrahuman provides the official source text or platform workflow.
