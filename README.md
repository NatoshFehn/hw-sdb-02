# Домашнее задание к занятию "Кеширование Redis/memcached" - Наталья Мартынова (Пономарева)

### Задание 1.

1. Слишком долгие транзакции, большое время отклика. Кеширование позволяет обеспечить доступ к часто запрашиваемым данным 
-долговременные сессии;
-веб-страницы;
-объекты, изображения, файлы, метаданные.
2. Большая нагрузка на основную базу данных (реляционную или NoSQL). Переиспользуем результаты частых запросов к БД из кэша.
3. Большое количество мелких I/O операций. 
4. Медленная потоковая передача мультимедиа. С помощью кеширования можно выполнять потоковую передачу видео миллионам пользователей одновременно.
5. Медленный антифрод или любой другой анализ данных с использованием Machine Learning. Кеширование позволяет проводить аналитику в реальном времени, предоставляет скоростное хранилище в памяти данных для моделей ML.
6. Оффлайн доступ. Кеширование позволяет приложениям работать без интернет-соединения, используя последние сохраненные данные (или часто используемые), но, разумеется, не все функции будут доступны в таком режиме.

В целом всё сводится к тому, что кеширование помогает ускорить работу приложений, веб-сервисов для клиентов, а также снизить нагрузку на бэкенд. Само по себе кеширование применяется практически везде, включая операционные системы, CDN, DNS, базы данных.

---

### Задание 2.

![Снимок1](https://github.com/NatoshFehn/hw-sdb-02/blob/main/Снимок1.png)

---

### Задание 3.

Добавила ключи key-1 и key-2 с произвольными значениями, при запросе значения через get они уже были удалены:  
![Снимок2](https://github.com/NatoshFehn/hw-sdb-02/blob/main/Снимок2.png)

Для примера добавила ключ-значение с TTL 15 и попробовала его запрашивать, через время он удалился:  
![Снимок3](https://github.com/NatoshFehn/hw-sdb-02/blob/main/Снимок3.png)  

---

### Задание 4.

Статус сервиса и проверка PING:  
![Снимок4](https://github.com/NatoshFehn/hw-sdb-02/blob/main/Снимок4.png)    

Запись в базу:  
![Снимок5](https://github.com/NatoshFehn/hw-sdb-02/blob/main/Снимок5.png)   

Чтение ключей в базе:  
![Снимок6](https://github.com/NatoshFehn/hw-sdb-02/blob/main/Снимок6.png)    

---
