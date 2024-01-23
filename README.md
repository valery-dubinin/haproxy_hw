# haproxy_hw
# Домашнее задание к занятию 2 «Кластеризация и балансировка нагрузки»

### Задание 1
- Запустите два simple python сервера на своей виртуальной машине на разных портах
- Установите и настройте HAProxy, воспользуйтесь материалами к лекции по [ссылке](2/)
- Настройте балансировку Round-robin на 4 уровне.
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

### Решение 1

Конфиг haproxy:

![img](https://github.com/valery-dubinin/haproxy_hw/blob/main/img/0.png)

Пример работы:

![img](https://github.com/valery-dubinin/haproxy_hw/blob/main/img/1.png)

Статистика:

![img](https://github.com/valery-dubinin/haproxy_hw/blob/main/img/2.png)

### Задание 2
- Запустите три simple python сервера на своей виртуальной машине на разных портах
- Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
- HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
- На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

### Решение 2

Конфиг haproxy:

![img](https://github.com/valery-dubinin/haproxy_hw/blob/main/img/3.png) 

Пример работы:

![img](https://github.com/valery-dubinin/haproxy_hw/blob/main/img/4.png)

Статистика:

![img](https://github.com/valery-dubinin/haproxy_hw/blob/main/img/5.png)
