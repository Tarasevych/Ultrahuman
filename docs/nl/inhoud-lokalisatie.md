# Voorstel voor lokalisatie van artikelen en aanbevelingen

**Taal:** Nederlands | [Українська (Oekraïens)](../uk/локалізація-вмісту.md) | [Naar afdelingsoverzicht](OVERZICHT.md) | [Naar hoofdpagina](../../LEESMIJ.nl.md)

Het statische taalpakket dekt de tekstonderdelen van de gebruikersomgeving voor Android en Compose. Artikelen, aanbevelingen, educatieve kaarten en andere leesteksten worden echter vaak vanuit de server of een inhoudsbeheersysteem aangeleverd, waardoor ze geen deel uitmaken van de statische programmabestanden.

## Aanbevolen werking van het product

Wanneer de taal van de gebruikersomgeving is ingesteld op Oekraïens (`uk` of `uk-UA`), dienen de toepassing en de achterliggende server Oekraïense teksten op te vragen zodra deze beschikbaar zijn:

- taalinstelling van de toepassing: `uk` of `uk-UA`;
- taalinstelling van het inhoudsbeheersysteem en de server: Oekraïens (`uk`);
- terugvaltaal: Nederlands of Engels wanneer een specifiek onderdeel nog niet in het Oekraïens beschikbaar is.

## Voorgestelde werkwijze

1. Exporteer de bronartikelen en aanbevelingen uit het officiële inhoudsbeheersysteem of de vertaalomgeving van Ultrahuman.
2. Lever de inhoud aan in Markdown, HTML, CSV, XLIFF, JSON of via een vertaalomgeving zoals Lokalise, Crowdin, Phrase of een ander intern hulpmiddel.
3. Vertaal de teksten aan de hand van dezelfde [woordenlijst](../../WOORDENLIJST.nl.md) die voor de gebruikersomgeving is toegepast.
4. Bewaak de medische en gezondheidsgerelateerde nuances zorgvuldig en vermijd overdreven gezondheidsclaims.
5. Importeer de gecontroleerde Oekraïense inhoud terug in het inhoudsbeheersysteem.
6. Controleer of Oekraïenstalige gebruikers de Oekraïense artikelen ontvangen en dat de terugvaltaal uitsluitend wordt getoond waar nog geen vertaling aanwezig is.

## Vrijwillige ondersteuning

De auteur van dit initiatief is graag bereid om kosteloos te helpen bij het vertalen en taalkundig nalopen van de Oekraïense inhoud zodra Ultrahuman de officiële bronteksten of toegang tot de vertaalomgeving beschikbaar stelt.
