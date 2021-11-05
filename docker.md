docker run -p 8888:8888 jupyter/scipy-notebook:33add21fab64 #создание юпитера для докера

docker exec -it 14e9a11a7ea8 bash # вход в контейнер

docker cp wine.data 14e9a11a7ea8:/home/jovyan/wine.data # копируем с локальной машины в докер

docker container kill 14e9a11a7ea8 # вырубаем контейнер

docker run -v C:\Users\ilyat\Desktop\Docker:/home/jovyan/ -p 8888:8888 jupyter/scipy-notebook:33add21fab64 # как сделать так, чтобы файлы оставались, даже если бы контейнер вырубался

docker build -t my_notebook . # опираясь на Dockerfile запускает то, что в нем

docker run -v C:\Users\ilyat\Desktop\Docker:/home/jovyan/ -p 8888:8888 my_notebook

docker-compose up # инфа выше (13ая строка) в один файл в качестве конфигурации

docker inspect df8f1e27ce3a #вся инф-ия про контейнер и ipшник

