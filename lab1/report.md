## **Цель работы:**
Изучить рабочую среду Cisco Packet Tracer, ознакомиться с интерфейсами основных устройств, типами кабелей, научиться собирать топологию. Изучить построение сети IP-телефонии с помощью маршрутизатора (2811), коммутатора и IP телефонов Cisco 7960 в среде Packet tracer  
## **Часть 1**  
Задание 1: Собрать схему соединения  
Смоделирована сеть (см. рисунок 1).

![Снимок](https://user-images.githubusercontent.com/17079352/223997682-a4aac116-375f-4e6a-8462-0a0b3e2af746.PNG))  
Рисунок 1 – Схема сети  

Задание 2: Настройка адресов
Каждому PC задан IP-aдрес в пределах 192.168.0.1 - 192.168.0.7 (см. рисунок 2).

![1 2](https://user-images.githubusercontent.com/59313334/221855971-f00ae491-d93e-4ba3-a3be-12b874eeecca.png)  
Рисунок 2 – Настройка адресов  

Проверена возможность отправки пакетов между участниками сети. Испытание прошло успешно (см. рисунки 3,4).

![image](https://user-images.githubusercontent.com/17079352/223998905-58b674e1-e380-4438-9317-8dbe1cfca2f8.png)
Рисунок 3 – Пинги из узла PC2 

![1 4(pc4)](https://user-images.githubusercontent.com/59313334/221856041-7a50af57-a94f-48c0-9687-5ba182ec2c8a.png)  
Рисунок 4 – Пинги из узла PC4    

## **Часть 2**  
Задание 1: Создание сети  
Спроектирована другая сеть с телефоными аппаратами (см. рисунок 5).  

![2 1](https://user-images.githubusercontent.com/59313334/221856104-a35d5b87-b453-4865-b617-ff9071b0e734.png)  
Рисунок 5 – Схема сети  

Задание 2: Настроить интерфейс роутера  
Задан ip адрес интерфейса роутера (см. рисунок 6)

![2 2](https://user-images.githubusercontent.com/59313334/221856197-ede7d54c-008d-477a-a06e-03758243412e.png)  
Рисунок 6 – Настройка интерфейса роутера  

Задание 3: Настройка IP-телефонии  
Для работы телефонов требуется подключить их к электрической сети (см. рисунок 7).
  
![2 3](https://user-images.githubusercontent.com/59313334/221856256-c23e1736-9ce2-4828-9b4e-cff37e33b4ba.png)  
Рисунок 7 – Подключение IP-телефона  

Конфигурация роутера:  
* Настроен dhcp сервер для автоматической адресации IP-телефонов сети, а также загружена прошивка для телефонов (см. рисунок 8).

	![2 4](https://user-images.githubusercontent.com/59313334/221856334-f022401a-63c8-4a17-bde4-f5f6cf464b00.png)  
	Рисунок 8 – Настройка DHCP для ip-телефонии  

* Заданы стандартные VoIP-параметры, такие как максимальное количество абонентов (см. рисунок 9).

	![2 5](https://user-images.githubusercontent.com/59313334/221856371-4c22b240-5783-484b-a31c-19d93e5f7cfd.png)  
	Рисунок 9 – Настройка параметров сети телефонов  

Конфигурация роутера закончена. Теперь настроим коммутатор:
* В нём vlan 1 выделен под VoIP (см. рисунок 10).

	![2 6](https://user-images.githubusercontent.com/59313334/221856400-304b5144-82dd-43ad-a544-83cfcfff3033.png)  
	Рисунок 10 – Конфигурация коммутатора  

Теперь в консоли роутера при помощи приведённых команд (см. рисунок 11) заданы устройствам телефонные номера.

![2 7](https://user-images.githubusercontent.com/59313334/221856426-8549d396-dc96-499b-8db9-6616bc1de3d6.png)  
Рисунок 11 – Назначение номеров телефонам	  

Произведена прозвонка с одного IP-телефона на другой. Эксперимент закончен с успешным результатом (см. рисунок 12).
	
![image](https://user-images.githubusercontent.com/17079352/224003244-1df1daf4-097e-4988-a7fd-73b99d4248d6.png)
Рисунок 12 – Успешное соединение

## **Вывод:**
В результате выполнения лаб.работы был освоен базовый функционал Cisco Packet Tracer, а также смоделирована функционирующая VoIP-сеть.
