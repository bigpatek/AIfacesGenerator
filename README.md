# AIfacesGenerator
Not ready yet. Using model for generating anime faces

### Архитектура проекта на стадии планирования:
![image](https://github.com/user-attachments/assets/bb07e0db-d4d2-493b-b673-9cc62dce606d)

* На данный момент есть каркас бота (без отправления запросов в очередь)
* Также уже есть обученная модель и осталось только прикрутить очередь, поднять контейнеры и залить на cloud.ru

Нейросеть берём с https://github.com/0x5eba/Anime-Character-Generator.git
Обучаем сами (директория с данными и сгенерированная модель отсутствуют в репозитории из-за веса. Гайд по обучению и всему что связано с нейросетью в директории network или по ссылке на оригинальный гитхаб)

Разворачиваем проект на cloud ru

Запуск
```
docker-compose build
docker-compose up -d rabbit_mq
docker-compose up -d bot
docker-compose up -d app
```
