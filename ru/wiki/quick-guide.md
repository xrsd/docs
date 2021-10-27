# Создать первую страницу

Попробуйте возможности {{ wiki-name }}, создав свою первую страницу. Страница будет создана в вашем личном разделе, так что не бойтесь экспериментировать.


## Создать страницу {#create}

Чтобы создать страницу в личном разделе:

1. [Перейдите на {{ wiki-name }}]({{ link-wiki }}) и на верхней панели нажмите кнопку **Создать**.

1. Заполните поле **Заголовок** и нажмите кнопку **Создать**.

    Поле с адресом заполняется автоматически. Не редактируйте его, если это ваша первая попытка создания страницы.

1. На левую панель скопируйте этот пример или придумайте свой:

    ```
    # Заголовок первого уровня
    ## Заголовок второго уровня
    Текст раздела.
    Пример [ссылки]({{ link-yandex }}).
    ### Заголовок третьего уровня
    *Текст выделен курсивом.* **Текст выделен полужирным.**
    ~~Зачеркнутый текст~~. `Фрагмент исходного кода`
    Маркированный список:
    * пункт списка;
      * подпункт;
      * подпункт.
    * пункт списка.

   Нумерованный список:
    1. Пункт списка.
    2. Пункт списка:
    3. Пункт списка.

    Пример таблицы:

    |header 1|header 2|header 3|
    |---|---|---|
    |cell 11|cell 12|cell 13|
    |cell 21|cell 22||
      ```

    {% cut "Как выглядит результат" %}

    ![](../_assets/wiki/example-wiki-page.png)

    {% endcut %}



1. Нажмите кнопку **Сохранить**.

Список всех ваших страниц доступен на верхней панели {{ wiki-name }} в меню **Закладки** → **Мои страницы**.

## Настроить доступ {#access}

Чтобы настроить доступ к вашей странице:

1. Перейдите на страницу.

1. Вверху страницы нажмите кнопку, на которой указан режим доступа к странице (по умолчанию **Доступно всем сотрудникам**).

1. Укажите, кто сможет просматривать страницу:

    - **Как у родительской страницы** — уровень доступа наследуется от родительской страницы.

    - **Все** — все сотрудники вашей организации.

    - **Только у авторов страницы** — только авторы могут просматривать и редактировать страницу.

    - **У некоторых сотрудников** — укажите логины пользователей, которым вы хотите открыть доступ для просмотра и редактирования.

    {% note warning %}

    Не рекомендуется изменять настройки доступа для [ главной страницы {{ wiki-name }}]({{ link-homepage }}).
    По умолчанию автором главной страницы {{ wiki-name }} является служебный аккаунт. Если для этой страницы выбран тип доступа «Только у авторов страницы», доступ для других пользователей будет заблокирован. Чтобы снять блокировку, перейдите по ссылке [ {{link-homepage-access}} ]({{ link-homepage-access }}) и измените параметры доступа.

    {% endnote %}

1. Нажмите кнопку **Сохранить**




