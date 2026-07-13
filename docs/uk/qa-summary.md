# QA summary

[English](../en/qa-summary.md)

Перед публікацією цього репозиторію були виконані автоматичні перевірки.

## Покриття

- Android strings: 3 597
- Android visible arrays: 4
- Android visible array items: 74
- Android plural resources: 10
- Ukrainian plural forms: 40
- Compose strings: 304

## Ukrainian quality audit

- Rows checked: 4 015
- Errors: 0
- Warnings: 0

Аудит перевіряє зламані форми Ring на кшталт `перстеньм`, помилковий переклад Ring як phone call, перекладений бренд Ultrahuman, literal John Doe placeholders, неправильний Clear, зламану HRV-граматику, русизми та ризики довжини compact labels.

## Ще потрібен human QA

Тільки Ultrahuman може повністю перевірити вміщення тексту в реальних signed app builds. Фінальний QA має покрити truncation, runtime strings, push notifications, server-driven content і доставку language split.
