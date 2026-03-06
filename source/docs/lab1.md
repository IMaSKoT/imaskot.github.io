# Лабораторная работа №1

## 1. Цель работы
- Освоить процесс создания статического сайта с использованием генератора документации MkDocs.   
- Научиться организовывать структуру документации проекта (портфолио лабораторных работ).   
- Изучить базовые принципы работы с системой контроля версий Git и платформой GitHub.   
- Развернуть статический сайт с использованием механизма GitHub Pages на домене вида username.github.io.   
- Освоить базовую настройку темы оформления и конфигурационного файла mkdocs.yml.   

## 2. Задание
1. Создать репозиторий.
2. Настроить MkDocs.
3. Написать отчеты и развернуть сайт.

## 3. Код 
Пример настройки `mkdocs.yml`:
```yaml
site_name: Портфолио
site_url: https://imaskot.github.io/demo/


theme:
  name: material
  language: ru
  palette:
    scheme: slate
    primary: black
    accent: deep-orange
  features:
    - navigation.tabs
    - header.autohide
    - content.code.copy


nav:
  - Обо мне: index.md
  - Лабораторные работы:
      - Введение: projects.md
      - Лабораторная 1: lab1.md
      - Лабораторная 2: lab2.md
  - Контакты: contact.md

plugins:
  - search
  - glightbox:
      touchNavigation: true
      loop: false
      effect: zoom
      slide_effect: slide

markdown_extensions:
  - admonition
  - pymdownx.details
  - pymdownx.superfences
  - pymdownx.highlight:
      anchor_linenums: true
      line_spans: __span
      pygments_lang_class: true
  - pymdownx.inlinehilite
copyright: Copyright &copy; 2026 Максим Седов
```

## 4. Выводы
В ходе выполнения лабораторной работы я успешно освоил генератор статических сайтов MkDocs, научился настраивать тему Material, работать с конфигурационным файлом `mkdocs.yml` и развернул готовое портфолио на платформе GitHub Pages.