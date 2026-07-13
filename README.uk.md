# Українська локалізація Ultrahuman

[English](README.md)

Це незалежні волонтерські матеріали української локалізації для Android-застосунку Ultrahuman.

Мета репозиторію - зробити внесок публічним, прозорим, зрозумілим для розробників і зручним для інтеграції командою Ultrahuman, якщо вони вирішать додати українську мову в одному з майбутніх релізів.

## Що включено

- Android-ресурси українською для `res/values-uk/`
- Український Compose resource file для `com.ultrahuman.algo.resources`
- Target-only CSV і JSON для перегляду або імпорту
- Інструкції інтеграції українською та англійською
- Пропозиція щодо локалізації статей, рекомендацій та серверного контенту
- Короткі QA-summary без робочих логів

## Чого тут немає

- Немає APK-файлів
- Немає витягнутих proprietary binaries
- Немає робочих логів і debugging artifacts
- Немає повної публічної таблиці англійських source-рядків застосунку

Публічні формати навмисно не перевидають повний англомовний текст застосунку. Тут є resource keys та український target-текст, щоб офіційна команда Ultrahuman могла зіставити ці матеріали зі своїм source project.

## Основні файли для інтеграції

```text
localization/android/res/values-uk/strings.xml
localization/android/res/values-uk/arrays.xml
localization/android/res/values-uk/plurals.xml
localization/android/res/xml/locales_config.xml
localization/composeResources/com.ultrahuman.algo.resources/values-uk/strings.commonMain.cvr
```

## Документація

- [Інструкція інтеграції](docs/uk/integration-guide.md)
- [Пропозиція щодо локалізації контенту](docs/uk/content-localization.md)
- [QA summary](docs/uk/qa-summary.md)
- [Текст звернення до Ultrahuman](docs/uk/outreach.md)
- [English documentation](docs/en/README.md)

## Покриття

- 3 597 Android string resources
- 4 видимі Android arrays / 74 array items
- 10 Android plural resources / 40 українських plural forms
- 304 Compose resource strings
- 4 015 рядків перевірено українським quality audit: 0 errors, 0 warnings

## Статус

Це не офіційний репозиторій Ultrahuman. Це волонтерський внесок користувача Ultrahuman, підготовлений для офіційного розгляду та можливої інтеграції.
