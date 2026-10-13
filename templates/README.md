# Шаблоны документирования аналитических задач (Yandex Wiki)

Локальные копии шаблонов из раздела [Управление аналитики](https://wiki.yandex.ru/upravlenie-analitiki/) на wiki.yandex.ru.

Расположение в репозитории: `ai_andoc/templates/`. Корень проекта: [../README.md](../README.md).

Дата выгрузки: 2026-10-13.

## Структура каталога

```
templates/
  skill/                         # шаблоны скилла napishi-dokumentaciyu
  analiticheskaya-podderzhka/    # канон для АП, каталог в .gitignore
  process/                       # трекер и регламент, каталог в .gitignore
  produktovaya-analitika/        # каталог в .gitignore
  operacionnaya-analitika/       # каталог в .gitignore
```

Шаблоны скилла лежат в [`skill/`](skill/). Остальные подкаталоги остаются локальными копиями и перечислены в [`.gitignore`](../.gitignore).

## Канон для аналитической поддержки

По странице [Как мы ведём аналитические задачи](https://wiki.yandex.ru/upravlenie-analitiki/onboarding/kak-my-vedjom-analiticheskie-zadachi) после завершения задачи обязательно документировать:

| Тип задачи | Файл в этой папке | Шаблон в wiki |
|------------|-------------------|---------------|
| Выгрузка | [analiticheskaya-podderzhka/vygruzka.md](analiticheskaya-podderzhka/vygruzka.md) | https://wiki.yandex.ru/_templates/3307/ |
| Исследование | [analiticheskaya-podderzhka/issledovanie.md](analiticheskaya-podderzhka/issledovanie.md) | https://wiki.yandex.ru/_templates/3304/ |
| Дашборд | [analiticheskaya-podderzhka/dashbord.md](analiticheskaya-podderzhka/dashbord.md) | https://wiki.yandex.ru/_templates/3305/ |
| A/B-тест | [analiticheskaya-podderzhka/ab-testy.md](analiticheskaya-podderzhka/ab-testy.md) | https://wiki.yandex.ru/_templates/3302/ |

Страницы `_templates/*` через API недоступны; тела шаблонов АП восстановлены по опубликованным копиям в wiki (операционная аналитика / УА) и по оглавлениям в [документации ПА лояльности](https://wiki.yandex.ru/upravlenie-analitiki/produktovaja-analitika-lojalnosti/dokumentacija-po-zadacham/shablony/).

## Постановка задачи в трекере

- [process/obshhij-shablon-opisaniya-zadachi-v-trekere.md](process/obshhij-shablon-opisaniya-zadachi-v-trekere.md)
- [process/kak-my-vedem-analiticheskie-zadachi.md](process/kak-my-vedem-analiticheskie-zadachi.md)

## Другие команды и контуры

| Файл | Источник в wiki |
|------|-----------------|
| [skill/shablon-dokumentirovaniya-kpa.md](skill/shablon-dokumentirovaniya-kpa.md) | Шаблон документирования задачи КПА. Его читает скилл |
| [produktovaya-analitika/korzina-vygruzka.md](produktovaya-analitika/korzina-vygruzka.md) | Шаблон документирования для Выгрузки (корзина) |
| [produktovaya-analitika/korzina-ab-test-kartochka.md](produktovaya-analitika/korzina-ab-test-kartochka.md) | Шаблон карточки теста (корзина) |
| [operacionnaya-analitika/poslednyaya-mila-ad-hoc.md](operacionnaya-analitika/poslednyaya-mila-ad-hoc.md) | Аналитика последней мили, ad-hoc |
| [operacionnaya-analitika/poslednyaya-mila-otchet.md](operacionnaya-analitika/poslednyaya-mila-otchet.md) | Аналитика последней мили, отчёты |
| [operacionnaya-analitika/kauzalnye-issledovaniya.md](operacionnaya-analitika/kauzalnye-issledovaniya.md) | Шаблон каузальных исследований |
| [skill/shablon-opisaniya-otcheta.md](skill/shablon-opisaniya-otcheta.md) | Шаблон описания отчёта (BI). Его читает скилл для разработки нового отчёта и для доработки отчёта. В таблице показателей есть колонка «Дата действия» |

## Именование страниц в wiki (ПА лояльность)

Формат названия статьи: `номер_задачи_в_ятеркере название` (пример: `PA-7531 Анализ перетоков`).

Репозитории Git для документирования перечислены на [странице «Шаблоны»](https://wiki.yandex.ru/upravlenie-analitiki/produktovaja-analitika-lojalnosti/dokumentacija-po-zadacham/shablony).
