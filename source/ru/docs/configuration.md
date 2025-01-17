---
title: Конфигурация
---
Можно изменить настройки в файле `_config.yml`.

### Сайт

Настройки | Описание
--- | ---
`title` | Название сайта
`subtitle` | Подзаголовок сайта
`description` | Описание сайта
`author` | Ваше имя
`language` | Язык сайта. Используйте [2-значный код ISO-639-1](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes). По умолчанию: `en`.
`timezone` | Временной пояс. Hexo использует настройки компьютера по умолчанию. Список доступных часовых поясов можно найти [здесь](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones). Несколько примеров: `America/New_York`, `Japan` и `UTC`.

### URL

Параметр | Описание | Умолчание
--- | --- | ---
`url` | URL-адрес сайта |
`root` | Корневая папка сайта |
`permalink` | [Постоянная ссылка](permalinks.html) используются ссылки на статьи | `:year/:month/:day/:title/`
`permalink_defaults` | Значение по умолчанию для каждого сегмента постоянной ссылки |

{% note info Сайт в подпапке %}
Если ваш сайт располагается в поддиректории (к примеру `http://example.org/blog`) поменяйте значение `url` на `http://example.org/blog` и установите переменной `root` значение `/blog/`.
{% endnote %}

### Папки

Параметр | Описание | Умолчание
--- | --- | ---
`source_dir` | Папка с исходниками. Здесь хранится контент | `source`
`public_dir` | Папка публикации. Здесь хранится сгенерированный сайт | `public`
`tag_dir` | Папка с тегами | `tags`
`archive_dir` | Папка с архивами | `archives`
`category_dir` | Папка с категориями | `categories`
`code_dir` | Папка с кодом | `downloads/code`
`i18n_dir` | Папка  i18n | `:lang`
`skip_render` | Пути, которые исключены из обработки. Можно использовать [глобальные выражения](https://github.com/micromatch/micromatch#extended-globbing) для определения путей |

### Написание

Параметр | Описание | Умолчание
--- | --- | ---
`new_post_name` | Имя файла для создания новых постов | `:title.md`
`default_layout` | Макет по умолчанию | `post`
`titlecase` | Преобразовать заголовки в заглавные буквы? | `false`
`external_link` | Открывать внешние ссылки в новой вкладке? | `true`
`external_link.enable` | Открывать внешние ссылки в новой вкладке? | `true`
`external_link.field` | Applies to the whole `site` or `post` only | `site`
`external_link.exclude` | Exclude hostname. Specify subdomain when applicable, including `www` | `[]`
`filename_case` | Преобразовать имена файлов в `1` нижний регистр; `2` верхний регистр | `0`
`render_drafts` | Отображать черновики? | `false`
`post_asset_folder` | Включать [папку с материалами](asset-folders.html)? | `false`
`relative_link` | Создание ссылок относительно корневой папки? | `false`
`future` | Отображать будущие посты? | `true`
`highlight` | Настройки блоков кода |
`highlight.enable` | Enable syntax highlight | `true`
`highlight.auto_detect` | Enable auto-detection if no language is specified | `false`
`highlight.line_number` | Display line number | `true`
`highlight.tab_replace` | Replace tabs by n space(s); if the value is empty, tabs won't be replaced | `''`

### Категории и теги

Параметр | Описание | Умолчание
--- | --- | ---
`default_category` | Категория по умолчанию | `uncategorized`
`category_map` | Карта категорий |
`tag_map` | Карта тегов |

### Даты / Времени формат

Hexo использует [Moment.js](http://momentjs.com/) для работы с датами.

Параметр | Описание | Умолчание
--- | --- | ---
`date_format` | Формат даты | `YYYY-MM-DD`
`time_format` | Формат времени | `HH:mm:ss`
`use_date_for_updated` | Use the date of the post in [`post.updated`](/ru/docs/variables#Переменные-страницы) if no updated date is provided in the front-matter. Typically used with Git workflow | `true`  

### Разбивка на страницы

Параметр | Описание | Умолчание
--- | --- | ---
`per_page` | Количество постов, отображаемых на странице. `0` отключает разбивку. | `10`
`pagination_dir` | Каталог разбивки | `page`

### Расширения

Параметр | Описание
--- | ---
`theme` | Имя темы. `false` отключает применение тем
`deploy` | Параметры публикации
