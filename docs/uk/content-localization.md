# Пропозиція щодо локалізації статей і рекомендацій

[English](../en/content-localization.md)

Static language pack покриває Android і Compose UI resources. Але статті, рекомендації, освітні картки й інший контент для читання можуть бути server-driven або CMS-driven, тому вони можуть не бути частиною APK resources.

## Рекомендована поведінка продукту

Коли мова інтерфейсу застосунку українська (`uk` / `uk-UA`), застосунок або backend мають запитувати український контент там, де він доступний:

- app locale: `uk` або `uk-UA`
- CMS/backend locale: Ukrainian
- fallback: English, якщо українського контенту ще немає

## Запропонований процес

1. Експортувати source articles/recommendations з офіційної CMS або localization platform Ultrahuman.
2. Надати контент у Markdown, HTML, CSV, XLIFF, JSON, Lokalise, Crowdin, Phrase або іншому внутрішньому форматі.
3. Перекладати з тим самим glossary, що й UI застосунку.
4. Обережно працювати з wellness/medical nuance і не перебільшувати обіцянки.
5. Імпортувати український контент назад у CMS.
6. Перевірити, що українськомовні користувачі отримують український контент, а English fallback використовується лише там, де потрібно.

## Волонтерська підтримка

Автор ініціативи готовий допомагати з перекладом і рев'ю українського контенту, якщо Ultrahuman надасть офіційний source text або workflow у localization platform.
