University: [ITMO University](https://itmo.ru/ru/) <br/>
Faculty: [FICT](https://fict.itmo.ru) <br/>
Course: IP-telephony <br/>
Year: 2022/2023 <br/>
Group: K34202 <br/>
Author: Perov Ivan <br/>
Lab: Lab4 <br/>
Date of create: 07.04.2023 <br/>
Date of finished: xx.04.2023 <br/>

# Лабораторная работа №4 "Построение сети ip-телефонии между удаленными маршрутизаторами"

## Ход выполнения
* Собрана топология сети, включающая в себя 2 маршрутизатора, 2 коммутатора, IP-телефоны и ПК в качестве конечных пользователей.
  
  ![image](https://user-images.githubusercontent.com/17079352/232143945-0a69ee4d-49b4-4505-8ee2-6c3a21d56c6e.png)

* Настроен интерфейс fa0/0 на каждом маршрутизаторе.
  
  ![image](https://user-images.githubusercontent.com/17079352/232144431-eceb0b1f-1ffc-4fa7-8897-f6c80d59fc2d.png)

* Настроены интерфейсы se1/0.
  
  ![image](https://user-images.githubusercontent.com/17079352/232144877-3c0e194e-43a6-4508-9a11-0d36245fe6a0.png)

* Настроен DHCP сервер.
  
  ![image](https://user-images.githubusercontent.com/17079352/232145763-ca4e7cec-4f3b-4bad-8e61-2b1890c24bef.png)

* Настроена динамическая маршрутизация RIP между маршрутизаторами.
  
  ![image](https://user-images.githubusercontent.com/17079352/232146383-626d1d4c-2f8b-460f-9804-9381ae660040.png)

* Настроен Cisco CallManager Express.
  
  ![image](https://user-images.githubusercontent.com/17079352/232146890-449a074f-08bf-497f-acee-44dd10e693bc.png)

* Сконфигурированы порты коммутаторов, а также указаны, что данные порты являются портами для доступа к vlan 1.
  
  ![image](https://user-images.githubusercontent.com/17079352/232147342-91cf5d74-a884-4d71-8071-94fa86af5e39.png)

* После всех настроек произведена проверка возможности вызова из одной сети в другую. Вызов прошел успешно.
  
  ![image](https://user-images.githubusercontent.com/17079352/232148202-78625653-4144-4080-a5de-e1fe2686b969.png)

## Выводы
В результате изучено построение связи нескольких сетей IP-телефонии.
