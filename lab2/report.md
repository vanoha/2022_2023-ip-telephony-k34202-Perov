University: [ITMO University](https://itmo.ru/ru/) <br/>
Faculty: [FICT](https://fict.itmo.ru) <br/>
Course: IP-telephony <br/>
Year: 2022/2023 <br/>
Group: K34202 <br/>
Author: Perov Ivan <br/>
Lab: Lab2 <br/>
Date of create: 20.03.2023 <br/>
Date of finished: 23.03.2023 <br/>

# Лабораторная работа №2 "Конфигурация voip в среде Сisco packet tracer"

## Описание
   Для выполнения данной лабораторной работы собирается схема соединения. Необходимо проверить, правильно ли подключены все узлы устройств. Предварительно удалить все преды- дущие конфигурационные файлы на маршрутизаторах Cisco 2811, на коммутаторе Cisco catalyst 3560.
   
## Цель работы:
   Изучить построение сети IP-телефонии с помощью маршрутизатора Cisco 2811, коммутатора Cisco catalyst 3560 и IP телефонов Cisco 7960.

## Ход работы:
   В процессе выполнения лабораторной работы были выпонены следующие шаги:
   
   ### Часть 1:
   1) Построена топология сети.
   
![image](https://user-images.githubusercontent.com/17079352/226307322-708245cf-b53b-427c-99f0-a1f4c339dbc6.png)

   2) Теперь поработаем в конфиге роутера.
      * В конфигурационном режиме изменено название маршрутизатора на CMERouter.<br/>
      * Отключен синтаксис ввода слов от DNS серверов
    
      * Заданы пароли для двух режимов: в удаленном режиме, в режиме консоли.
  
        ![image](https://user-images.githubusercontent.com/17079352/226308296-c4fb51e7-5f17-40a2-9944-4d10e6d1b089.png)
  
      * Для возможности передавать данные настроен интерфейс fa0/0 на CMERouter.

        ![image](https://user-images.githubusercontent.com/17079352/226310858-86081234-8261-4131-96e5-a3354e0c1dbe.png)

      * Для передачи голоса и данных на CMERouter настроен DHCP. Также настроены услуги телефонии Cisco CallManager Express.
  
        ![image](https://user-images.githubusercontent.com/17079352/226312204-7334e4b8-134a-42c5-b373-027d70715334.png)
        ![image](https://user-images.githubusercontent.com/17079352/226312598-4be420d3-4bdc-4ea6-bb85-76a85e97995d.png)
  
  3) Чуть позже еще вернемся к настройке маршрутизатора. Теперь обратимся к коммутатору:
  
      * На коммутаторе созданы VLAN порты для взаимодействия коммутатора с маршрутизатором и подключены IP телефоны. Настроены IP-телефоны и соединены с коммутатором.
      * Чтобы удостоверится, что верно всё настроено, проверены звонки между телефонами.

        ![image](https://user-images.githubusercontent.com/17079352/226330642-06b592c8-cb21-403a-9baa-ffc68e885ee9.png)

   ### Часть 2:
   1) Продолжим настройку коммутатора:
      * Созданы VLAN порты на коммутаторе и настроено подключение IP телефонов.

        ![image](https://user-images.githubusercontent.com/17079352/227185664-de6f967c-f2b8-42c0-899e-3e21af04dead.png)

      * Задан маршрут по умолчанию командой, а также настроен порт (тип trunk).

        ![image](https://user-images.githubusercontent.com/58363643/226112598-75ce35b5-f08c-4c6b-8f40-a748ca83aabf.png)

   2) Вернемся к роутеру:
      * Финальная стадия: настроен DHCP сервер, подключен и настроен Call Manager Express, а также настроены IP телефоны.

        ![image](https://user-images.githubusercontent.com/58363643/226112906-b977ef34-fcde-4bee-998c-33581fd1fada.png)
        ![image](https://user-images.githubusercontent.com/58363643/226112948-3a83d206-fb2b-4e05-a39b-703e1d18853e.png)

        ![image](https://user-images.githubusercontent.com/17079352/227186705-f940f108-6db8-46ec-b957-a771e4eafd53.png)

   3) Результат проверки работы:

      <img src="https://user-images.githubusercontent.com/58363643/226121168-eead5dc4-1a2b-4818-8ab7-a731ca25aad1.png" width="400">
      ![image](https://user-images.githubusercontent.com/17079352/227189346-38c94e3b-a2e0-49c6-b9f1-c651ab945fbf.png)

## Выводы:
Таким образом, была изучена схема настройки IP-телефонии с помощью CallManager Express.
