# Інструкція інтеграції

[English](../en/integration-guide.md)

## 1. Додати Android-ресурси українською

Додайте українські ресурси в Android-модуль, де вже лежать базові `res/values/` ресурси:

```text
app/src/main/res/values-uk/strings.xml
app/src/main/res/values-uk/arrays.xml
app/src/main/res/values-uk/plurals.xml
```

Файли в цьому репозиторії:

```text
localization/android/res/values-uk/strings.xml
localization/android/res/values-uk/arrays.xml
localization/android/res/values-uk/plurals.xml
```

## 2. Зареєструвати українську локаль

Перевірена версія застосунку вже має:

```xml
android:localeConfig="@xml/locales_config"
```

Потрібно додати українську:

```xml
<locale android:name="uk" />
```

Готовий приклад файлу:

```text
localization/android/res/xml/locales_config.xml
```

## 3. App Bundle / language split

Встановлений Android-пакет уже використовує language splits, наприклад нідерландську через `split_config.nl.apk`. Після додавання `values-uk` і `uk` у locale/build config pipeline App Bundle має змогти створити український language split.

## 4. Додати Compose resources

У застосунку також є Compose resources у `composeResources/com.ultrahuman.algo.resources`. Додайте:

```text
localization/composeResources/com.ultrahuman.algo.resources/values-uk/strings.commonMain.cvr
```

Це відповідає вже наявній структурі `values-nl`, `values-pl` та інших мов.

## 5. Альтернативи для імпорту

Якщо команда користується localization platform, доступні target-only формати:

```text
formats/csv/*.csv
formats/json/*.json
```

Публічний репозиторій навмисно не містить повних англійських source-string workbooks. Команда Ultrahuman може зіставити переклад за resource keys у своєму офіційному source project.

## 6. Обов'язковий фінальний QA

Перед релізом Ultrahuman варто перевірити українську в signed internal build:

- вміщення тексту в кнопках, картках, діалогах, графіках, Ring setup і сповіщеннях;
- server-driven/runtime рядки, яких немає у static resources;
- доставку language split через Google Play;
- відповідність тону бренду Ultrahuman.

Волонтерський автор готовий продовжити QA після ввімкнення української в test build або production rollout.
