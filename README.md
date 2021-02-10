# Project MMM
---
## Работа с RFiD

Для читывание информации с карты используем файл Read.py
А для записи карточки в массив используем Write.py

## Работа с MAX30102
Для считывании информации с датчика мы используем 4 файла
max30102.py - служит для подключения датчика по i2c в нем задаються адреса и параметры работы датчика
hrcalc.py - используется для перевода значений приходящих с i2c в температуру целсия
heartrate_monitor.py - этот файл используется как сбор информации в массивы данных 
```sh
BPS = [] #массив с данными пульса 25 значений 
SPO2 = [] #массив с данными уровня кислорода 25 значений 
```
## Работа с GY906
Для считывания температуры с данного датчика мы используем файл Temp-gy906.py
Когда мы считываем температуру мы можем посмотреть температуру снаружи и на обьекте который присланен к датчику:
Команда для считывание температуры вокруг.
```sh
sensor.get_ambient()
```
Команда для считывание температуры с обьекта который показан.
```sh
sensor.get_object_1()
```