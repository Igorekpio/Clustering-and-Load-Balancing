# Домашнее задание к занятию 2 «Кластеризация и балансировка нагрузки»

### Задание 1
- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

# Решение
#### Конфигурационный файл HAproxy
https://github.com/Igorekpio/Clustering-and-Load-Balancing/blob/main/haproxy4.cfg
![image](https://github.com/user-attachments/assets/6c0fbf4c-0b77-4ddb-bc55-54ec262e5bba)


### Задание 2
- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

# Решение  
#### Конфигурационный файл HAproxy
https://github.com/Igorekpio/Clustering-and-Load-Balancing/blob/main/haproxy7.cfg
![image](https://github.com/user-attachments/assets/a09a051d-cd18-4c64-be16-9d85956074ce)
