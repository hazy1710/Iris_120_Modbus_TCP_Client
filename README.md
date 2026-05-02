# Iris_120_Modbus_TCP_Client
Это клиент для подключения к щитовому прибору ИРИС-120 по Modbus-TCP. Приложение опрашивает регистры (напряжения, тока и частоты) ИРИС-120 через Modbus-TCP и выводит их на экран.

Так как проект Electron имеет внушительный размер, здесь размещены только ключевые файлы.

Проект разработан с использованием фреймворка [Electron](https://www.electronjs.org/ru/docs/latest/) - это фреймворк для разработки десктопных приложений с использованием HTML, CSS и JavaScript. А также [node-modbus](https://github.com/Cloud-Automation/node-modbus) — это простой клиент/сервер Modbus TCP/RTU с простым API.

Подготовка
------------

Для компиляции проэкта вам понадобятся:

1. Установить [Git](https://github.com/git-guides/install-git).

2. [Node.js](https://nodejs.org/en/download) и входящий в ее состав менеджер пакетов npm.

Сборка
------------
Инициализация npm проекта и установка Electron, модуля node-modbus.
```
mkdir my-electron-app && cd my-electron-app
npm init
npm install electron --save-dev
npm install jsmodbus
```
Скопировать файл настроек datafile.db и папку src в корень проекта.

Открыть блокнотом datafile.db и указать IP-адрес/порт Modbus-TCP устройства к которому подключен ИРИС-120.

Выполнить
```
npm run start
```
