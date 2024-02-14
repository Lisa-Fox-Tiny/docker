## Сборка образа
docker build ./ --tag pagination:0.0.1
## Запуск контейнера
docker run --name my_pagination -d -p 8000:8000 pagination:0.0.1
