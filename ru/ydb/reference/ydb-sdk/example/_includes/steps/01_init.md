---
sourcePath: ru/ydb/ydb-docs-core/ru/core/reference/ydb-sdk/example/_includes/steps/01_init.md
---
## Создание экземпляра драйвера, клиента и сессии {#driver-client-session-init}

Для взаимодействия с {{ ydb-short-name }} необходимо создать экземпляр драйвера, клиента и сессии:

* Драйвер {{ ydb-short-name }} отвечает за взаимодействие приложения и {{ ydb-short-name }} на транспортном уровне. Драйвер должен существовать на всем протяжении жизненного цикла работы с {{ ydb-short-name }} и должен быть инициализирован перед созданием клиента и сессии.
* Клиент {{ ydb-short-name }} работает поверх драйвера {{ ydb-short-name }} и отвечает за работу с сущностями и транзакциями.
* Сессия {{ ydb-short-name }} содержит информацию о выполняемых транзакциях и подготовленных запросах и содержится в контексте клиента {{ ydb-short-name }}.