# aiq-final — Launch Readiness Assessment

Дмитро Суга́к · PayPilot / Verta · стан **11.11.2026, після L10**.

Це окремий документ рішення, **не завершена фінальна здача**. [LRA](lra.md) і [Evidence Map](evidence-map.md) заповнюються поступово. Усі використані вимірювання — власні прогони навчального стенду; походження окремих кейсів із курсу не перетворює результати на запасний артефакт. Дані не є production-статистикою.

## Документи і статус

| Документ | Стан |
| --- | --- |
| [lra.md](lra.md) | Робоча версія: відповіді на питання 1–5 та блок рішення; 6 після L13, 7 після L11/L14 |
| [evidence-map.md](evidence-map.md) | Числа, наслідки й обмеження поточної LRA з посиланнями на незмінні версії ДЗ |
| [board-brief.md](board-brief.md) | Шаблон до листа CEO після L14; ліміт 2 сторінки |
| [incident-postmortem.md](incident-postmortem.md) | Шаблон до листа Compliance і картки після L14; ліміт 1,5 сторінки |
| [answers.md](answers.md) | Шаблон до питань ментора; відповідь протягом 2 днів, до 150 слів на питання |

## Репозиторії ДЗ — джерела, не копії

Нумерація ДЗ відрізняється від номерів занять. У фіналі немає коду, датасетів, звітів, трейсів чи git-історії попередніх ДЗ. Старі репозиторії не змінювались цією підготовкою. Кожне доказове посилання в Evidence Map фіксує повний commit SHA, а не рухому `main`.

| Теми | ДЗ / джерело | Зафіксована версія | Що беремо |
| --- | --- | --- | --- |
| L01–L02 | [ДЗ1 — Quality Bar](https://github.com/Dmitriy004/paypilot-l02-quality-bar) | [2a13c7a](https://github.com/Dmitriy004/paypilot-l02-quality-bar/tree/2a13c7a6790158195eadf9bfd061d8f7c98ea29e) | Контракт L01 зафіксований у §0–1 прийнятого ДЗ після L02; окремого public ДЗ L01 не заявляємо |
| L03 | [ДЗ2 — Golden Suite](https://github.com/Dmitriy004/paypilot-l03-golden-suite) | [c470cd3](https://github.com/Dmitriy004/paypilot-l03-golden-suite/tree/c470cd3d4d6c965cf8b509593437a666b0ab6c7d) | Межі набору й залишковий ризик |
| L04 | [ДЗ3 — Retrieval Diagnostic](https://github.com/Dmitriy004/paypilot-l04-ragas-diagnostic) | [dcba9b9](https://github.com/Dmitriy004/paypilot-l04-ragas-diagnostic/tree/dcba9b98511c41cded75d391e6a6f7576d5c5cad) | Джерело / пошук / формування відповіді |
| L05 | [ДЗ4 — Multi-turn](https://github.com/Dmitriy004/paypilot-l05-multiturn) | [71d3b76](https://github.com/Dmitriy004/paypilot-l05-multiturn/tree/71d3b766baa95daa7496c884facdf597fc1f2a76) | Втрата фактів розмови, контроль і повтори |
| L06 | [ДЗ5 — Security](https://github.com/Dmitriy004/paypilot-hw05-security) | [3d000b4](https://github.com/Dmitriy004/paypilot-hw05-security/tree/3d000b44910e7ee4cb5b1a297148ee950fd21669) | Перечитаний журнал атак, відтворені та невідтворені ланки |
| L07 | [ДЗ6 — Tool Calls](https://github.com/Dmitriy004/paypilot-hw06-tool-calls) | [47f6103](https://github.com/Dmitriy004/paypilot-hw06-tool-calls/tree/47f61039c23f0bffdffe6e9ceae512d47656d413) | Фактичні записи, незворотні дії, виміряні прототипи перевірок |
| L08 | [ДЗ7 — Observability](https://github.com/Dmitriy004/paypilot-hw07-observability) | [300c457](https://github.com/Dmitriy004/paypilot-hw07-observability/tree/300c4578b32cf268eaa3fe45b4bf9d17fcfd11af) | Перечитаний трейс-розбір, ціна і незалежна звірка витрат |
| L09 | [ДЗ8 — Judge Trust](https://github.com/Dmitriy004/paypilot-hw08-judge-trust) | [0637cfa](https://github.com/Dmitriy004/paypilot-hw08-judge-trust/tree/0637cfae7ac50a85b78a2160771cfc847de85eb3) | Довіра до автоматичної оцінки та її похибка |
| L10 | [ДЗ9 — Local Judge](https://github.com/Dmitriy004/paypilot-hw09-local-judge) | [dc76f55](https://github.com/Dmitriy004/paypilot-hw09-local-judge/tree/dc76f55924abb574ec60d05ae33a657321717a68) | Локальна оцінка: якість, час, гроші й межі периметра |
| L11–L14 | Поки немає завершених джерел у цій підготовці | — | Додати після відповідних робіт; не видавати заплановане за виконане |

## Шаблони і майбутня здача

Офіційна [сторінка шаблонів GoIT](https://www.edu.goit.global/uk/learn/53575439/54507480/55543754/training?blockId=55620604). У [templates/](templates/) перенесені всі поля й заголовки п'яти шаблонів; зміст не заповнений. У робочій Evidence Map колонка «Документ» поки містить LRA та підготовку до майбутніх документів — це не твердження про вже написаний бриф.

Після L14: прочитати обидва листи й картку, відтворити саме заданий інцидент, написати короткі документи, додати докази червоного і зеленого CI-прогонів після L13. За правилами курсу бриф, postmortem і відповіді ментору перед здачею потребують особистої переробки автора; поточна робоча LRA не є його фінальним схваленням.

## Постзадача після кожного курсового завдання

[Обов'язковий checklist](post-task-checklist.md) та [правила репозиторію](AGENTS.md). Додатково локально збережена scoped інструкція у глобальному `~/.codex/AGENTS.md`, щоб застосовувати цей крок і під час роботи в інших репозиторіях PayPilot. Це правило виконання, не фонове спостереження й не автоматична здача.

[Звірка джерел та прочитане L06/L08](docs/sources-and-verification.md). Висновки цієї підготовки не стверджують встановлених production-виправлень чи відтворення фінальної картки інциденту.
