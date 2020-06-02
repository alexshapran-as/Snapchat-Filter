# Обнаружение и распознавание сигналов. Домашнее задание. Вариант 2. Маски Snapchat
------------

# Установка
```sh
python3 -m virtualenv -p python3 .env
source .env/bin/activate
pip3 install -r requirements.txt
(mkdir -p resources; cd resources; curl http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2 | bzip2 -d > shape_predictor_68_face_landmarks.dat)

```

# Запуск
```sh
source .env/bin/activate

# Glasses filter
./main.py --filter glasses --footage <path to glasses.png>
# Moustache filter
./main.py --filter moustache --footage <path to moustache.png>

```

# Дополнительно

После клонирования репозитория и установки зависимостей создайте в корне проекта папку "resources". 
В ней расположите предварительно обученные данные для лиц, которые доступны по ссылке:
http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2
