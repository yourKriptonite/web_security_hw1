## Cделано
- [x] Проксирование HTTP запросов 5 баллов
- [x] Проксирование HTTPS запросов 5 баллов
- [x] Отправка сохраненного запроса 5 баллов

## Как запустить

Требуются порты 8080, 8081, 5432
```
docker-compose up --build
```
Запросы проксируются через порт 
```
8080
```
Переключение между http и https осуществляется за счет параметра main.schema в configs/config.yaml
```
  schema: "http" #switch to https if you want
```

## Работа с repeater-ом
Список сохранненых реквестов
```
http://localhost:8081/requests
```
Повтор реквеста
```
http://localhost:8081/<id>
```