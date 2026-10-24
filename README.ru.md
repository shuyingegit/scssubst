[English](README.md) · [中文](README.zh-CN.md) · [日本語](README.ja.md) · [한국어](README.ko.md) · [Español](README.es.md) · [Français](README.fr.md) · [Deutsch](README.de.md) · **Русский**

<p align="center">
  <img src="docs/banner.svg" alt="ScsSubst" width="100%">
</p>

<h1 align="center">ScsSubst</h1>

<p align="center">
  <strong>Папки в буквы дисков</strong><br>
  Дайте глубокой папке букву диска — без копирования, как локальный диск.
</p>

<p align="center">
  <a href="https://subst.scsoi.com"><img src="https://img.shields.io/badge/Website-subst.scsoi.com-0F766E?style=flat-square" alt="Website"></a>
  <a href="https://github.com/shuyingegit/scssubst/releases/latest"><img src="https://img.shields.io/github/v/release/shuyingegit/scssubst?style=flat-square&label=Release" alt="Release"></a>
  <a href="https://subst.scsoi.com/#download"><img src="https://img.shields.io/badge/Windows-10%20%2F%2011-0078D4?style=flat-square&logo=windows&logoColor=white" alt="Windows"></a>
  <a href="mailto:support@scsoi.com"><img src="https://img.shields.io/badge/Support-support%40scsoi.com-6B7280?style=flat-square" alt="Support"></a>
</p>

<p align="center">
  <a href="https://subst.scsoi.com/#download"><strong>Скачать</strong></a> ·
  <a href="https://subst.scsoi.com/#pricing"><strong>Цены</strong></a> ·
  <a href="https://github.com/shuyingegit/scssubst/releases"><strong>Releases</strong></a> ·
  <a href="https://drive.scsoi.com"><strong>ScsDriver</strong></a>
</p>

---

## Зачем ScsSubst?

Дайте глубокой папке букву диска — без копирования, как локальный диск.

Инструменты могут писать и удалять — боитесь, что затронут лишнее? Диск, с которого они не выйдут.

<p align="center">
  <img src="docs/hero.png" alt="ScsSubst hero" width="920">
</p>

## Для чего подходит

- Частые папки → буквы дисков
- Держать инструменты на одном диске
- Укоротить длинные пути проектов
- По диску на рабочую зону

### Важно: более безопасный песочничный рабочий диск

**Диск, с которого оно не выйдет**

Когда ПО может широко писать и удалять, риск — выйти за рамки. Сопоставьте папку букве диска и держите инструмент на нём.

1. Отдельная рабочая папка
2. Буква диска (напр. Z:)
3. Workspace инструмента на Z:

> Workspace инструмента на этом диске. Практическая изоляция, не OS-песочница.

<p align="center">
  <img src="docs/sandbox-usecase.png" alt="ScsSubst sandbox use case" width="920">
</p>

## Основные функции

Просто, стабильно, без лишних хлопот.

- **Монтирование в один клик** — Выберите папку и букву, нажмите «Подключить» — по желанию снова при запуске приложения.
- **Нативный опыт** — В проводнике как обычный диск — короче пути.
- **Автозапуск** — Можно снова подключить сохранённые профили при открытии ScsSubst.
- **Лёгкий и стабильный** — Только API Windows — без стороннего драйвера. Компактная portable-сборка.
- **Несколько сопоставлений** — Добавляйте несколько папок, у каждой своя буква.
- **Доп. параметры** — Видимость для elevated-приложений, корзина и т.д. По умолчанию просто.
- **Пробный период после установки** — 7 дней; затем лицензия (месяц / год / бессрочно).
- **Песочничный диск** — Пишущие инструменты часто выходят за рамки и удаляют не то. Назначьте отдельную папку букве диска и укажите инструменты туда.


## Скачать

Последние сборки: **[GitHub Releases](https://github.com/shuyingegit/scssubst/releases/latest)** · [Сайт](https://subst.scsoi.com/#download)

| Пакет | Когда использовать |
|--------|----------|
| **Portable (`.zip`)** | Распаковать и запустить (рекомендуется) |
| **Installer (`.exe`)** | Установщик |

Системные требования: Windows 10 / 11 (64-бит)

## Цены

Пробный период начинается с 7 дней. Пригласите друга — продлить можно обоим.

Все тарифы (включая бесплатный период) включают техподдержку: при ошибке или проблеме напишите нам — разберёмся, исправим и будем улучшать.

## Смежный продукт

Подключите WebDAV / облако как локальный диск Windows.

→ **[ScsDrive](https://github.com/shuyingegit/scsdriver)** · [drive.scsoi.com](https://drive.scsoi.com)

## Частые вопросы

**Чем отличается от облачного монтирования?**  
ScsSubst сопоставляет папки на ПК. Для облака/WebDAV используйте ScsDriver (drive.scsoi.com).

**В чём разница между пробной и лицензионной версией?**  
Функции те же. Пробный период 7 дней; с кодом друга — 14. Если кто-то начнёт пробный период с вашим кодом, вы тоже получите +7 дней без ограничения. Бессрочные лицензии дни не добавляют. После окончания нужна лицензия.

**Как использовать ScsSubst как безопасную песочницу?**  
Создайте отдельную рабочую папку, сопоставьте букву диска и укажите workspace инструмента туда. Случайные удаления останутся на диске. Это не OS-песочница.

## Лицензия и условия

Условия · Конфиденциальность · Возврат — [https://subst.scsoi.com/terms](https://subst.scsoi.com/terms) · [https://subst.scsoi.com/privacy](https://subst.scsoi.com/privacy) · [https://subst.scsoi.com/refund](https://subst.scsoi.com/refund)

---

<p align="center">
  <a href="https://subst.scsoi.com/"><strong>Открыть сайт →</strong></a>
</p>
