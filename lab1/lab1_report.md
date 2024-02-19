University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [IP-telephony](https://github.com/itmo-ict-faculty/ip-telephony)

Year: 2023/2024

Group: K34212

Author: Gomzyakov Alexander Nikolaevich

Lab: Lab1

Date of create: 19.02.2024

Date of finished: 19.02.2024

# Отчет по лабораторной работе №1 "Базовая настройка ip-телефонов в среде Сisco packet tracer" #

## Цель работы ##
Изучить рабочую среду Cisco Packet Tracer, ознакомить- ся с интерфейсами основных устройств, типами кабелей, научиться собирать топологию. Изучить построение сети IP-телефонии с помощью маршрутизатора, коммутатора и IP телефонов Cisco 7960 в среде Packet tracer

## Ход работы ##

### 1 Часть ###

Первым делом соберем топологию сети по примеру:
![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/0cc8f86f-c5a7-4e52-9a5e-2b00f56c3ff6)

После выдадим каждому компьютеру в сети уникальный ip-адрес 192.168.0.1/24 - 192.168.0.7/24

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/09e2797f-61ad-46f8-a73a-ce6035bda898)

Проверим передачу пакетов с компьютера одного свитча до компьютера другого свитча с помощью команды ping.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/95eb8522-af2f-4f50-8059-396e3c5663d7)

### 2 Часть ###

Первым делом соберем топологию сети по примеру:

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/302b90ec-8c21-4768-a5a8-43a7c7a81d1b)

Далее изменим имя маршрутизатора на CMERouter

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/705dfb81-42c6-4f5b-b66f-30f24cb14a8b)

После этого настроим интерфейс fa0/0 на маршрутизаторе Cisco 2811 (CMERouter)

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/cd1175a6-d907-49ca-bdb6-93823cd3d208)

Теперь настроим DHCP сервера для передачи голоса и данных на маршрутизаторе - Cisco 2811

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/c915d798-13ef-4c2e-bc24-f6423edc3c94)

Далее Настроим услуги телефонии Cisco CallManager Express на маршрутизаторе 2811

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/a249bf2d-3f2e-4ae3-8559-d29da98855f0)

Теперь создадим VLAN порты на коммутаторе для взаимодействия коммутатора с маршрутизатором и подключить IP телефоны.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/b22c6691-a603-4aa7-b3f5-ebe0f19b4398)

Подключим телефоны в сеть

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/5e27581e-303c-4e56-91a4-cd20a061c8f6)

Выдадим номера телефона 

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/71f11363-bb71-42f0-87be-98715f724f20)

Попробуем подключиться с одного телефона к другому.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/686d481f-f82a-43ca-b04d-e3ac52f6ea44)

## Вывод ##
В результате выполнения лабораторной работы получилось настроить 2 топологии сети. В первой мы настроили и пропинговали компьютеры, во-второй у нас получилось позвонить с одного телефона на другой. 



