# Домашнее задание к занятию "`Использование Ansible`" - `Маркин Алексей`

## Основная часть

1. Допишите playbook: нужно сделать ещё один play, который устанавливает и настраивает LightHouse.
2. При создании tasks рекомендую использовать модули: `get_url`, `template`, `yum`, `apt`.
3. Tasks должны: скачать статику LightHouse, установить Nginx или любой другой веб-сервер, настроить его конфиг для открытия LightHouse, запустить веб-сервер.
4. Подготовьте свой inventory-файл `prod.yml`.
5. Запустите `ansible-lint site.yml` и исправьте ошибки, если они есть.

![Вопрос5](https://github.com/Markin-AI/ans-03/blob/main/img/5.png)

6. Попробуйте запустить playbook на этом окружении с флагом `--check`.
7. Запустите playbook на `prod.yml` окружении с флагом `--diff`. Убедитесь, что изменения на системе произведены.
8. Повторно запустите playbook с флагом `--diff` и убедитесь, что playbook идемпотентен.

![Вопрос8](https://github.com/Markin-AI/ans-03/blob/main/img/8.png)

![Вопрос8](https://github.com/Markin-AI/ans-03/blob/main/img/9.png)

![Вопрос8](https://github.com/Markin-AI/ans-03/blob/main/img/10.png)

9. Подготовьте README.md-файл по своему playbook. В нём должно быть описано: что делает playbook, какие у него есть параметры и теги.

10. Готовый playbook выложите в свой репозиторий, поставьте тег `08-ansible-03-yandex` на фиксирующий коммит, в ответ предоставьте ссылку на него.

[ссылка на коммит](https://github.com/Markin-AI/ans-03/commit/9ed19244d174cb039e48269a1a7d2c80354cf2ea)

---