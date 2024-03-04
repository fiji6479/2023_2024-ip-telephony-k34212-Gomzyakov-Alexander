University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [IP-telephony](https://github.com/itmo-ict-faculty/ip-telephony)

Year: 2023/2024

Group: K34212

Author: Gomzyakov Alexander Nikolaevich

Lab: Lab3

Date of create: 04.03.2024

Date of finished: 04.03.2024

# Отчет по лабораторной работе №3 "Использование Asterisk в качестве SIP proxy" #

## Цель работы ##

Изучить программный комплекс Asterisk. Настройка Asterisk для локальных звонков.

## Ход работы ##

Первым делом установим Asteriks в операционной системе ubuntu.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/eb46de63-d4a1-476d-881e-a714cede3193)

После этого изменим файл sip.conf для того, чтобы добавить номера телефонов.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/4348afcb-4cc2-4751-b63f-bb9d0264cef2)

Также изменим файл extensions.conf. Добавим в нем схему маршрутизации.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/ff11875d-aa3d-4b04-9654-ab8e1e9f362a)

После перезапуска изменения вступят в силу.

Теперь установим и настроим аккаунт в приложении Zoiper5

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/8415d816-9686-4420-af24-b29d0ebb3eb9)

После этого установим утилиту wine (она позволяет устанавливать приложения win на linux)

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/7f8be8e7-aadf-4bb7-8614-7e63dfbbb99f)

Теперь с помощью утилиты wine установим приложение MicroSIP.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/376c31f5-54ec-49c9-bcd2-e68a52be43a7)

Следующим шагом настроим приложение MicroSIP.

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/773b9ac3-b8f8-4241-9f53-4c57cd4ef97b)

Теперь попробуем позвонить с Zoiper5 на MicroSIP

![изображение](https://github.com/fiji6479/2023_2024-ip-telephony-k34212-Gomzyakov-Alexander/assets/71012423/3cd3d601-70f0-46bf-9fee-3e0afb22a4de)

В итоге мы получили звонокна приложении MicroSIP и успешно ответили.

## Вывод ##
В ходе выполнения работы мы успешно настроили Zoiper и MicroSIP. Также успешно настроили конфиг Asteriks и маршрутизацию.
