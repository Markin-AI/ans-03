# Install Clickhouse and Vector Ansible Playbook

Плейбук для установки Clickhouse, Vector, Lighthouse, ОС Linux использующих пакетный менеджер на базе rpm.

## Конфигурация

Файл конфигурации:
`./group_vars/clickhouse/vars.yml`

Переменные:

`clickhouse_version:` - версия clickhouse
`clickhouse_packages:` - список пакетов для установки

Файл конфигурации:
`./group_vars/vector/vars.yml`

Переменные:

`vector_version:` - версия vector
`vector_architecture:` - системная архитектура пакета vector

Файл конфигурации:
`./group_vars/lighthouse/vars.yml`

Переменные:

`lighthouse_vcs:` -  исходный код
`lighthouse_location:` расположение Lighthouse

## Установка

Запуск плейбука:

```bash
sudo ansible-playbook -i inventory/prod.yml site.yml
```

## Play Tags

clickhouse - Для установки clickhouse

vector - Для установки vector

nginx - Для установки nginx

Lighthouse - Для установки lighthouse

## Templates:

Файл шаблона:

`./templates/vector.j2`

Файл содержит базовую конфигурацию Vector в формате yaml и устанавливается на целевой хост при запуске плейбука.

`./templates/nginx.j2`

Файл содержит базовую конфигурацию nginx в формате yaml и устанавливается на целевой хост при запуске плейбука.

`./templates/lighthouse.j2`

Файл содержит базовую конфигурацию lighthouse в формате yaml и устанавливается на целевой хост при запуске плейбука.