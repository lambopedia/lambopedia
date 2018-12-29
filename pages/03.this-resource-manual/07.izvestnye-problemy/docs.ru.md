---
title: 'Известные проблемы'
---

## Сертификат защищённого соединения
1. Используется бесплатный сертификат от Let’s Encrypt сроком на 3 месяца. Проблема в автопродлении - пока никто не сделал скрипт по расписанию, который бы продлевал нам сертификат.
2. Некоторые страницы открываются по-старому, через незащищённое соединение. Почему? - непонятно, никто не разбирался ещё с этим.

## Сохранение настроек
При сохранении настроек слетает используемая тема - с доработанной (ExtLearn) на базовую (Learn). Почему? - непонятно, никто не разбирался ещё с этим. Поэтому после внесения каких-либо изменений, убедитесь что активна доработанная тема ExtLearn, именно с помощью неё реализован поиск и доработки внешнего оформления.

## GitSync
В коде синхронизации наличие изменений определяется через ответ от программы Git, которая установлена на сервере (вроде как на любом Linux-сервере). Ответ приходит в виде строки. И сравнивается со строкой. На нашем сервере при запросе ответа на английском, ответ всё-равно приходит на русском. Я добавил в код небольшое исправление, благодаря которому ответ приходит на английском. Предложил изменение в GitHub в проекте GitSync. Если его не примут, то следующее обновление плагина GitSync нужно делать осторожно, иначе он перестанет работать. А именно - необходимо сделать резервную копию, обновиться, и если исправления в обновлении нет - добавить его снова.  