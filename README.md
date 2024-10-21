# Ansible роли для мониторинга и логирования

Этот проект содержит набор Ansible ролей для установки и конфигурации Prometheus, Node Exporter, ElasticSearch, Kibana и FluentBit. Проект предназначен для разворачивания служб мониторинга и логирования вне Kubernetes, с возможностью сбора системных логов и метрик.

## Содержание

- **Prometheus**: Установка и настройка для мониторинга хостов, включая самого Prometheus.
- **Node Exporter**: Установка и добавление метрик хоста в Prometheus.
- **ElasticSearch и Kibana**: Установка и запуск стека для хранения и визуализации логов.
- **FluentBit**: Установка и настройка сбора системных логов из journald и отправка их в ElasticSearch.

## Как использовать

1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com/roman-domanchuk/ansible-monitoring-logging
    ```

2. Перейдите в каталог проекта:
    ```bash
    cd ansible-monitoring-logging
    ```

3. Запустите playbook:
    ```bash
    ansible-playbook playbook.yml
    ```

## Требования

- Ansible 2.9+
- Python 3.6+

## Структура проекта

- `roles/` — Каталог с Ansible ролями.
- `playbook.yml` — Основной playbook для выполнения всех ролей.
- `inventory.ini` — Инвентарь с хостами для развертывания.
- `ansible.cfg` — Конфигурационный файл Ansible.
