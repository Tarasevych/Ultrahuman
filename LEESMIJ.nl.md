# Oekraïense lokalisatie voor Ultrahuman

**Taal:** Nederlands | [Українська (Oekraïens)](ОГЛЯД.uk.md) | [Tweetalig overzicht (README.md)](README.md)

Dit zijn onafhankelijke, vrijwillig vervaardigde materialen voor de Oekraïense lokalisatie van de Ultrahuman-toepassing op Android.

Het doel van deze opslagplaats is om de bijdrage openbaar, transparant, inzichtelijk en eenvoudig integreerbaar te maken voor de ontwikkelaars van Ultrahuman, mochten zij besluiten om ondersteuning voor de Oekraïense taal toe te voegen in een toekomstige uitgave.

## Wat is inbegrepen

- Oekraïense bronbestanden voor Android onder `res/values-uk/`
- Oekraïens taalbestand voor Compose onder `com.ultrahuman.algo.resources`
- Uitwisselingsbestanden met uitsluitend doelteksten in CSV- en JSON-formaat voor beoordeling of import
- Integratiegidsen in het Oekraïens en het Nederlands
- Voorstel voor het lokaliseren van artikelen, gezondheidsaanbevelingen en servergestuurde inhoud
- Beknopte samenvatting van de kwaliteitscontrole zonder interne werklogboeken
- Geharmoniseerde woordenlijst voor medische en technische termen

## Rechtstreeks bekijken zonder downloaden

- [Pakket-index](docs/nl/pakket-index.md)
- [XML-bronbestanden voor Android](localization/android/res/values-uk/)
- [Taalbestanden voor Compose](localization/composeResources/com.ultrahuman.algo.resources/values-uk/)
- [CSV-exportbestanden met doelteksten](formats/csv/)
- [JSON-exportbestanden met doelteksten](formats/json/)
- [Rapport van de kwaliteitscontrole (JSON)](qa/summary.json)

## Wat niet is opgenomen

- Geen installatiebestanden (`APK`)
- Geen geëxtraheerde afgesloten programmabestanden
- Geen interne werklogboeken of foutopsporingsbestanden
- Geen openbare tabel met de volledige oorspronkelijke bronteksten van de toepassing

De openbare bestanden vermijden bewust het herpubliceren van de volledige brontekst van de toepassing. Enkel de sleutelnamen en de Oekraïense doelteksten zijn opgenomen, zodat het officiële team van Ultrahuman deze materialen rechtstreeks kan koppelen aan het eigen bronproject.

## Belangrijkste bestanden voor integratie

```text
localization/android/res/values-uk/strings.xml
localization/android/res/values-uk/arrays.xml
localization/android/res/values-uk/plurals.xml
localization/android/res/xml/locales_config.xml
localization/composeResources/com.ultrahuman.algo.resources/values-uk/strings.commonMain.cvr
```

## Documentatie

- [Overzicht van de Nederlandse documentatie](docs/nl/OVERZICHT.md)
- [Pakket-index](docs/nl/pakket-index.md)
- [Integratiegids](docs/nl/integratiegids.md)
- [Voorstel voor lokalisatie van inhoud](docs/nl/inhoud-lokalisatie.md)
- [Samenvatting van de kwaliteitscontrole](docs/nl/kwaliteitscontrole-samenvatting.md)
- [Contactbericht aan het team](docs/nl/contactbericht.md)
- [Woordenlijst](WOORDENLIJST.nl.md)
- [Oekraïense documentatie](docs/uk/ОГЛЯД.md)

## Dekking

- 3.597 Android-tekstreeksen
- 4 zichtbare Android-tekstlijsten / 74 lijstonderdelen
- 10 Android-meervoudsreeksen / 40 Oekraïense meervoudsvormen
- 304 Compose-tekstreeksen
- 4.015 rijen gecontroleerd door de Oekraïense taalkwaliteitscontrole: 0 fouten, 0 waarschuwingen

## Status

Dit is geen officiële opslagplaats van Ultrahuman. Het betreft een vrijwillige bijdrage van een Oekraïenstalige gebruiker van Ultrahuman, voorbereid voor officiële beoordeling en mogelijke integratie.
