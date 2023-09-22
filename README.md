# instruction-docker-app


# Шаг 1: Файл должен быть сохранен как docker-compose.yml в любой директории на вашем компьютере.
Скачайте его с данного репозитория
# Шаг 2: Перейдите в директорию, где находится ваш docker-compose.yml файл:
```bash
cd <путь/до/директории>
```
# Шаг 3: Запуск всех контейнеров:
```bash
docker-compose up
```
Если вы хотите запустить контейнеры в фоновом режиме, добавьте флаг -d:

```bash
docker-compose up -d
```
Этот файл и команды запустят все три образа как контейнеры, сделав их доступными на соответствующих портах. Контейнер с базой данных Postgres будет зависим от переменных окружения для имени базы данных, имени пользователя и пароля.

Дополнительно:
Для остановки всех контейнеров выполните:

```bash
docker-compose down
```
Для обновления всех образов с Docker Hub:

```bash
docker-compose pull
```

# Проверка работоспособности приложений
## Запущены ли контейнеры
![image](https://github.com/Postman33/instruction-docker-app/assets/20001037/2dc567e9-1eee-422c-8816-938a4ea28aae)

## Проверить доступность сервера(playground graphql) по 3000 порту:
Проверялось по URL: [http://localhost:8000/](http://localhost:3000/graphql) или http://localhost:3000
![image](https://github.com/Postman33/instruction-docker-app/assets/20001037/13a16243-13ed-4306-b3bf-c7f88c492c3e)

## Проверить доступность клиент-приложения на Svelte по 8000 порту
Проверялось по URL: http://localhost:8000/
![image](https://github.com/Postman33/instruction-docker-app/assets/20001037/773a05ef-3d7e-4c55-99c2-a487f6a32347)


