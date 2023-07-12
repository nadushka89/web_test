# Тестирование веб-приложений  семинары №3


## Урок 3. Инструменты прокси трафика

Формат сдачи: PDF или скрин вашего дз (для каждого спсоба замены по три скрина: UI до замены, скрин настройки способа замены из charles, UI после замены - итого 9 скринов на замену и 2 скрина на пункт 6 дз - 1 скрин с настройками Throttle Settings и 1 скрин с UI что получилось +описать словами) - все скрины должны располагаться на вашем гуглдиске - онлайн - в качестве дз - присылайте ссылку на гуглдиск (дз в формате rar-zip-exel-doc со скачиванием на локальную машину не могут быть приняты к проверке)
1. Необходимо настроить Charles Proxy
2. Найти запрос на https://test-stand.gb.ru/gateway/users/profile/user_id (открыть Профиль)
3. Подменить в ответе на свои данные:
1. firstName
2. lastName
3. username
4. phone
5. status
6. sex
7. birthDate
8. updatedAt
4. Необходимо выполнить подмену тремя способами: Rewrite/Breakpoint/Map Local
5. В качестве ответа - необходимо сделать скриншот подмен (все три способа на скриншоте должно быть видно charles proxy с подменой + что отображается на вебе в профиле)
6. Необходимо настроить Throttle Settings, выставив значения только для хоста test-stand.gb.ru и выставить Bandwidth - download: 10, upload: 10 - обновить страницу профиля и проверить как будет долго выполняться запрос и ответить на вопрос, выполнится ли запрос или нет.

**Задание:**

Breakpoint:

!["До"](https://github.com/nadushka89/web_test/blob/main/source/1_breakpoint.png)

!["После"](https://github.com/nadushka89/web_test/blob/main/source/2_breakpoint.png)

!["скрин настройки способа замены из charles"](https://github.com/nadushka89/web_test/blob/main/source/3_breakpoint.png)

Rewrite:

!["До"](https://github.com/nadushka89/web_test/blob/main/source/1_rewrite.png)

!["После"](https://github.com/nadushka89/web_test/blob/main/source/2_rewrite.png)

!["скрин настройки способа замены из charles"](https://github.com/nadushka89/web_test/blob/main/source/3_rewrite.png)

Map local:

!["До"](https://github.com/nadushka89/web_test/blob/main/source/1_maplocal.png)

!["После"](https://github.com/nadushka89/web_test/blob/main/source/2_maplocal.png)

!["скрин настройки способа замены из charles"](https://github.com/nadushka89/web_test/blob/main/source/3_maplocal.png)


Throttle:

Выполнится ли запрос или нет? Запрос не выполнится,так как слишком маленький максимальный объем данных,который может быть передан с течением времени

![](https://github.com/nadushka89/web_test/blob/main/source/throttle.png)

![](https://github.com/nadushka89/web_test/blob/main/source/throttle2.png)