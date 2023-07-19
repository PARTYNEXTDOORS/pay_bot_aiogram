
____

<h1 align="left" id="macropower-title">Телеграм бот для приема платежей</h1>

____

## Описание проекта:
Простенький телеграм бот для приема платежей (в моем случае через платежный шлюз сбербанка)

____

## Запуск проекта на локально сервере
Для начала стоит [создать бота](https://chatlabs.ru/botfather-instrukcziya-komandy-nastrojki/) и подключить бота к платежам, например [юкасса](https://yookassa.ru/docs/support/payments/onboarding/integration/cms-module/telegram).
+ склонировать репозиторий
```
git clone git@github.com:PARTYNEXTDOORS/pay_bot_aiogram.git
```
+ установить вирутиальное окружение
```
python -m venv venv`(для Windows)
python3 -m venv env`(для Mac/Linux)
```
+ активировать виртуальное окружение
```
source venv/Script/activate`(для Windows)
source venv/bin/activate`(для Mac/Linux)
```
+ установаить бибилиотеку aiogram
```
pip install aiogram
```
+ установить библиотеку pyqiwip2p
```
pip install pyQiwiP2P
```
+ в файле `config.py` ввести token бота и платежного шлюза, который вы выбрали (если вы собираетесь выкладывать бота в открытый доступ, не забудьте перенести токены в файл `.env`, чтобы скрыть токены)
+ запустить код
```
python main.py
```
