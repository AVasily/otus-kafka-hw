
Домашнее задание

Запуск Kafka
Цель:

Научиться самостоятельно запускать Kafka (быстрый старт).

Описание/Пошаговая инструкция выполнения домашнего задания:

Самостоятельно запустить Kafka по предложенному алгоритму:

    Установить Java JDK
    Скачать Kafka с сайта kafka.apache.org и развернуть на локальном диске
    Запустить Zookeeper
    Запустить Kafka Broker
    Создать топик test
    Записать несколько сообщений в топик
    Прочитать сообщения из топика
    В материалах к этому занятию можете найти видеоинструкцию по сдаче ДЗ.



ui
http://localhost:9000/

создать топик
kafka-topics --bootstrap-server kafka1:9191 --create --topic test --replication-factor 1 --partitions 3

отправить сообщение
kafka-console-producer --bootstrap-server kafka1:9191 --topic test

прочитать сообщение
kafka-console-consumer --bootstrap-server kafka1:9191 --topic test --group testuser --from-beginning

дополнительные ресурсы
https://github.com/OtusTeam/OTUS-Kafka
https://github.com/Magnusyatina/kafka-homework/tree/master/hw1