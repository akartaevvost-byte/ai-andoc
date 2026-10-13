# ai_andoc

Локальные артефакты для документирования аналитических задач.

## Шаблоны (Yandex Wiki)

Копии шаблонов из раздела [Управление аналитики](https://wiki.yandex.ru/upravlenie-analitiki/): каталог [`templates/`](templates/) и оглавление [`templates/README.md`](templates/README.md).

| Путь | Назначение |
|------------|------------|
| `templates/shablon-*.md` | Два шаблона в корне `templates/`, которые читает скилл |
| `templates/analiticheskaya-podderzhka/` | Обязательные типы документации АП (выгрузка, исследование, дашборд, A/B). Каталог в `.gitignore` |
| `templates/process/` | Постановка задачи в трекере и регламент ведения. Каталог в `.gitignore` |
| `templates/produktovaya-analitika/` | Шаблоны корзины. Каталог в `.gitignore` |
| `templates/operacionnaya-analitika/` | Последняя миля, каузальные исследования. Каталог в `.gitignore` |

## Скилл

Скилл `napishi-dokumentaciyu` лежит в [`.agents/skills/napishi-dokumentaciyu/`](.agents/skills/napishi-dokumentaciyu/SKILL.md). Его подхватывают Cursor, Claude Code и Antigravity, включая окно и терминал `agy`, когда открыт этот репозиторий.

Скилл стартует, когда ты пишешь «Напиши документацию» или «Напиши документацию по задаче». В Cursor и Claude Code ту же работу запускает команда `/napishi-dokumentaciyu`.

Скилл предлагает шаблон и записывает документ после твоего согласия. Для большинства задач он предлагает [`templates/shablon-dokumentirovaniya-kpa.md`](templates/shablon-dokumentirovaniya-kpa.md). Шаблон [`templates/shablon-opisaniya-otcheta.md`](templates/shablon-opisaniya-otcheta.md) он предлагает для разработки нового отчёта и для доработки отчёта. В доработке скилл берёт прежнее описание за основу. Если меняется логика метрики, старая строка помечается как неактуальная с датой, до которой она действовала, а у новой логики в колонке «Дата действия» стоит дата, с которой она действует. Новый сеанс нужен, чтобы среда увидела скилл после его появления.
