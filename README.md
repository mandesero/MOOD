# MOOD - monster multiplayer adventure


## Сборка
```
git clone https://github.com/mandesero/MOOD.git
cd MOOD
pip install pipenv
pipenv shell
pipenv install -d
pipenv sync
```

### Генерация документации по серверу
```
doit html
```
см. *MOOD/\_build/html/index.html*

### Создание wheel-пакетов
```
doit wheels
```
*wheel-пакеты находятся в MOOD/moodserver/dist/ и MOOD/moodclient/dist/*

## Установка wheel-пакетов (Server)
В чистом окружении 
```
pip install <path-to-server-wheel>
```

### Запуск сервера
```
StartServer
```

## Установка wheel-пакетов (Client)
В чистом окружении 
```
pip install <path-to-client-wheel>
```

### Запуск клиента
```
StartClient <login>
```

## Игра (Client)
### доступные команды
  - up, down, right, left - перемещение по полю
  - addmon \<monster_name> hello \<hello_phrase> hp \<hp> coords \<x> \<y> - добавляет монстра *monster_name* в точку *(x, y)* на поле, который говорит *hello_phrase* и имеет *hp* здоровья
  - attack \<monster_name> (attack \<monster_name> with \<gun>) - атака монстра *monster_name* (возможен выбор оружия *gun*)
  - sayall \<message> - отправка сообщения другим игрокам на карте
  - locale ru_RU.UTF8 - смена языка на русский




