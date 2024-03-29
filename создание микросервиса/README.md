Создание микросервиса

Цель работы
Познакомиться с механизмом работы современных веб-приложений и микросервисной архитектуры в процессе выполнения творческого задания.

Задания для выполнения
На основе предложенного шаблона реализуйте сервис, реализующий регистрацию пользователей. Сервис должен поддерживать REST API и коллекцию /user/, хранящую данные о логинах и паролях пользователей, зарегистрированных в системе. Сервис должен принимать и отдавать информацию в формате JSON. Сервис должен хранить следующую информацию про каждого пользователя: логин, хеш пароля (лучше с солью), дату регистрации.

Настройте веб-сервер по Вашему выбору (Apache2 или nginx) таким образом, чтобы он поддерживал соединение по протоколу HTTPS. Для этого сгенирируйте самоподписанный сертификат SSL.

Модифицируйте код вашего сервиса таким образом, чтобы он поддерживал защищенное соединение.

На основе предложенного шаблона реализуйте сервис, реализующий регистрацию пользователей. Сервис должен поддерживать REST API и коллекцию /user/, хранящую данные о логинах и паролях пользователей, зарегистрированных в системе. Сервис должен принимать и отдавать информацию в формате JSON. Сервис должен хранить следующую информацию про каждого пользователя: логин, хеш пароля (лучше с солью), дату регистрации.

Для тестирования используется пакет requests, который производит  различные запросы. При хэшировании пароля в начало поля password добавляется соль, чтобы в будущем при реализации авторизации пользователя ее можно было легко получить. При попытке создать двух разных пользователей с одинаковым паролем, результат получается разный благодаря добавлению соли. При удалении пользователя сервер не возвращает ничего, поэтому строка ответа сервера пустая. При попытке создать пользователя с уже существующим именем или при попытке получить информацию о несуществующем пользователе сервер отдает сообщение с ошибкой.

![image](https://user-images.githubusercontent.com/70269164/146627290-e9c08c6f-aab1-4447-a935-464202fdf360.png)

![image](https://user-images.githubusercontent.com/70269164/146627293-78581a10-4f32-4eb3-b6d8-5777a9cc8281.png)

![image](https://user-images.githubusercontent.com/70269164/146627295-0764de2a-5878-4c54-8093-3a3856b6117c.png)

Настройте веб-сервер по Вашему выбору (Apache2 или nginx) таким образом, чтобы он поддерживал соединение по протоколу HTTPS. Для этого сгенирируйте самоподписанный сертификат SSL.

![image](https://user-images.githubusercontent.com/92279258/146290831-bb514de3-89ca-41c9-9f7a-66f2763f9bd3.png)

![image](https://user-images.githubusercontent.com/92279258/146290698-c01a5e81-5c44-4b39-98fb-9ed4786d7f4d.png)

![image](https://user-images.githubusercontent.com/92279258/146290727-5c690bc7-50d8-4df0-8679-73ca19c33436.png)

![image](https://user-images.githubusercontent.com/92279258/146290894-821c01b6-406d-4096-aea4-8b0fce3979e7.png)

![image](https://user-images.githubusercontent.com/92279258/146290909-12e9f2cf-603e-4cda-92da-500ac8d75ae3.png)

Модифицируйте код вашего сервиса таким образом, чтобы он поддерживал защищенное соединение.

![image](https://user-images.githubusercontent.com/70269164/146627302-19cbd93b-5741-4f21-98c0-1c47ccb67b3f.png)

![image](https://user-images.githubusercontent.com/70269164/146627304-87ea3cb5-fd04-490b-a6c9-c9085c44e9d0.png)

![image](https://user-images.githubusercontent.com/92279258/146291050-8fefca3d-9bc3-4a0b-8c67-046615d02dca.png)


