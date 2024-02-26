University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [IP-telephony](https://github.com/itmo-ict-faculty/ip-telephony)

Year: 2023/2024

Group: K34212

Author: Gomzyakov Alexander Nikolaevich

Lab: Lab2

Date of create: 26.02.2024

Date of finished: 26.02.2024

# Отчет по лабораторной работе №2 "Конфигурация voip в среде Сisco packet tracer" #

## Цель работы ##
Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

## Ход работы ##

### 1 Часть ###
Первым делом соберем топологию сети по примеру:

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/98531c81-77b2-4bc0-a35f-740c9df94432)

Далее в конфигурационном режиме изменим название маршрутизатора на CMERouter.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/624bfb23-e232-4482-9c1d-956c2843b19f)

Для того чтобы отключить синтаксис ввода слов от DNS серверов выполним следующую команду:

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/478a7df4-4329-4b27-ba6e-dc19975ce25c)

Зададим пароли для защиты маршрутизатора как в удаленном режиме, так и в режиме консоли.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/6e7c7e3e-0533-401c-9e93-0e63b4dfeda4)

Теперь настроим интерфейс fa0/0 на маршрутизаторе Cisco 2811 (CMERouter)

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/de2cfa56-0472-4244-8b79-5689ced3a206)

Следующим шагом Настроим DHCP сервера для передачи голоса и данных на маршрутизаторе Cisco 2811.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/caeca547-d8b9-4432-9e56-a1fe9f9fba8b)

Настроим услуги телефонии Cisco CallManager Express на маршрутизаторе 2811

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/bf475d13-8f24-4f49-b542-cb210b8c6d6d)

Далее создадим VLAN порты на коммутаторе Cisco Catalyst 3560 для взаимодействия коммутатора с маршрутизатором и подключить IP телефоны.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/aac4657a-bcb1-42ca-850c-a30a18a388c1)

Теперь настроим телефоны и выдадим им номера.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/02a9885d-5707-4587-8eef-4b197f50243a)

Проверим работоспособность

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/091f5ce6-185a-41e4-b380-d17473af92ce)

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/d939b519-2666-4095-ac4e-4a195017158c)

### 2 Часть ###

