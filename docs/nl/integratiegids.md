# Integratiegids

**Taal:** Nederlands | [Українська (Oekraïens)](../uk/посібник-інтеграції.md) | [Naar afdelingsoverzicht](OVERZICHT.md) | [Naar hoofdpagina](../../LEESMIJ.nl.md)

## 1. Oekraïense bronbestanden voor Android toevoegen

Voeg de Oekraïense taalbestanden toe aan de Android-module waarin de bestaande standaardbestanden onder `res/values/` zich bevinden:

```text
app/src/main/res/values-uk/strings.xml
app/src/main/res/values-uk/arrays.xml
app/src/main/res/values-uk/plurals.xml
```

Overeenkomstige bestanden in deze opslagplaats:

```text
localization/android/res/values-uk/strings.xml
localization/android/res/values-uk/arrays.xml
localization/android/res/values-uk/plurals.xml
```

## 2. Oekraïense taalcode registreren

De onderzochte versie van de toepassing bevat reeds de volgende verwijzing:

```xml
android:localeConfig="@xml/locales_config"
```

Voeg hier de Oekraïense taalcode aan toe:

```xml
<locale android:name="uk" />
```

Een uitgewerkt voorbeeld van dit configuratiebestand is opgenomen onder:

```text
localization/android/res/xml/locales_config.xml
```

## 3. Toepassingsbundel en taalsplitsing

Het geïnstalleerde Android-pakket maakt reeds gebruik van afzonderlijke taalbundels, bijvoorbeeld voor het Nederlands via `split_config.nl.apk`. Zodra de map `values-uk` aanwezig is en `uk` is opgenomen in de taalinstellingen van het bouwproces, kan de bouwpijplijn automatisch een Oekraïense taalbundel aanmaken.

## 4. Compose-taalbestanden toevoegen

De toepassing bevat daarnaast taalbestanden voor Compose onder `composeResources/com.ultrahuman.algo.resources`. Voeg daar het volgende bestand aan toe:

```text
localization/composeResources/com.ultrahuman.algo.resources/values-uk/strings.commonMain.cvr
```

Deze indeling sluit naadloos aan op bestaande taalmappen zoals `values-nl`, `values-pl` en andere ondersteunde talen.

## 5. Alternatieve formaten voor import

Indien het ontwikkelteam gebruikmaakt van een vertaalbeheersysteem, zijn er bestanden met enkel de sleutelnamen en de Oekraïense doelteksten beschikbaar:

```text
formats/csv/*.csv
formats/json/*.json
```

Deze openbare opslagplaats bevat bewust geen volledige tabellen met de oorspronkelijke bronteksten van de toepassing. Het team van Ultrahuman kan de vertalingen eenvoudig op basis van de sleutelnamen koppelen binnen het officiële bronproject.

## 6. Aanbevolen eindcontrole vóór uitgave

Vóór de officiële uitgave wordt aanbevolen om de Oekraïense weergave in een ondertekende interne testversie te controleren:

- tekstlengte en plaatsing in knoppen, kaarten, dialoogvensters, grafieken, schermen voor ringinstelling en meldingen;
- servergestuurde teksten en dynamische meldingen die niet in de statische bronbestanden zijn opgenomen;
- juiste uitlevering van de afzonderlijke taalbundel via Google Play;
- aansluiting van de schrijfstijl bij de merktoon van Ultrahuman.

De vrijwillige bijdrager staat klaar om de eindcontrole voort te zetten zodra het Oekraïens in een testversie of gefaseerde uitrol wordt ingeschakeld.
