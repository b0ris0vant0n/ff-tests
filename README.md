# Как тестировать свои разработки

## Цели
1. Проект ff запланирован быть большим и сложным. Человек способен у себя в голове уместить 5 вещей одновременно на различных уровнях абстракции. FF будет сложнее. Следовательно невозможно будет вручную самому проверить новый и старый функционал на корректное и некорректное поведение. Необходим инструмент, который поможет разработчикам автоматически проверять весь проект.
2. Код-ревью подразумевает под собой проверку написанного кода в статичном формате. Для этого ревьюеру необходимо на цифрах и фактах убедиться, что новый код работает и старый код работает. Нужен соответствующий инструмент для этого. 
3. Необходимо не ломать данные на различных контурах (прод | дев). Для этого до данных этих двух контуров никто не имеет доступ.
 
## Решения

### Для разработки 
1. просить backend разработчика поднимать локально свой API с помощью [ngrok](https://ngrok.com/) [tutorial](https://www.youtube.com/watch?v=NrSS6TCBP-Y)
2. использовать openapi.json для использования в качестве a) документации, b) основы для мокового сервера (api, который отдает данные согласно документации, но с рандомными данными) [что такое openapi](https://habr.com/en/articles/776538/) [как достать openapi.json из api (просто перейти по https://<api_url>/openapi.json)](https://fastapi.tiangolo.com/reference/openapi/docs/) [как фронту поднять моковый сервер на основе openapi.json](https://nuvolar.medium.com/build-a-mock-rest-api-with-swagger-ui-using-open-api-specification-and-docker-4665b53b8d85) [mock server 2](https://medium.com/@angela.tt/efficient-tools-for-generating-mockserver-from-openapi-spec-and-tracking-changes-a2424bb0ebfc)

### Для тестирования

#### Документации

1. [nextjs tests](https://nextjs.org/docs/app/building-your-application/testing)
2. [react](https://ru.legacy.reactjs.org/docs/testing.html)

#### Доклады

1. [автоматизация браузерного тестирования без бэкенда с помощью Playwright](https://youtu.be/U1IsDZVVNho?si=qvUkSLNytiLZkDUM)
2. [моки данных для фронтенда: как сделать эффективно и востребованно](https://youtu.be/7fsDNAUXBUA?si=OXssFBkqv5_pif80)
3. [хорошие UI-тесты, реально?!](https://youtu.be/FeCOpE3s1Wo?si=-eqkIT5GEWDwL_bA)
4. [тестирование современного фронтенда (самокат)](https://youtu.be/_HM76ktNcTA?si=e5IJ0eqazzEGeljl)
5. [дизайн и унификация UI-тестов на базе Model Based Testing (ВТБ)](https://youtu.be/edF36htB7CQ?si=5P3TryPU4pd23p3o)
