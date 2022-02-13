# 3.6 Компьютерный сети
## 1.
        Код ответа 200
"Успешно". Запрос успешно обработан
## 2.
Рис 1
Рис 2
## 3.
2ip.ru

188.243.183.194.pool.sknt.ru

## 4.
Скайнет

        origin:         AS35807
## 5.
       $ traceroute -An 8.8.8.8
        traceroute to 8.8.8.8 (8.8.8.8), 30 hops max, 60 byte packets
        1  192.168.88.1 [*]  9.091 ms  9.105 ms  9.325 ms
        2  * * *
        3  * * *
        4  * * *
          * * *
        6  * 185.37.128.142 [AS35807]  11.861 ms  12.371 ms
        7 185.37.128.106 [AS35807]  12.442 ms  10.325 ms  13.051 ms
        8  72.14.216.110 [AS15169]  29.425 ms  30.388 ms  30.478 ms
        9  * * *
        10  209.85.245.238 [AS15169]  76.763 ms 74.125.244.129 [AS15169]  77.703 ms 209.85.245.238 [AS15169]  77.182 ms
        11  74.125.244.181 [AS15169]  77.926 ms 74.125.244.133 [AS15169]  78.087 ms 74.125.244.180 [AS15169]  78.066 ms
        12  142.251.51.187 [AS15169]  8.684 ms 72.14.232.85 [AS15169]  7.351 ms 72.14.232.84 [AS15169]  23.945 ms
        13  142.251.61.219 [AS15169]  14.386 ms 172.253.64.55 [AS15169]  27.096 ms 142.250.209.171 [AS15169]  30.245 ms
        14  216.239.63.25 [AS15169]  33.345 ms * 172.253.51.237 [AS15169]  35.661 ms
        и т.д. 

## 6.
Wrst — максимальное время задержки;
Рис 4
## 7.
        dig +trace @8.8.8.8  dns.google.com
        1 шаг 8.8.8.8
        2 шаг e.root-servers.net
        3 шаг h.gtld-servers.net
        4 шаг ns1.google.com
## 8.
        dig -x 216.239.32.10 (Любой IP адрес)

        ; <<>> DiG 9.16.1-Ubuntu <<>> -x 216.239.32.10
        ;; global options: +cmd
        ;; Got answer:
        ;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 51860
        ;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

        ;; OPT PSEUDOSECTION:
        ; EDNS: version: 0, flags:; udp: 65494
        ;; QUESTION SECTION:
        ;10.32.239.216.in-addr.arpa.	IN	PTR

        ;; ANSWER SECTION:
        10.32.239.216.in-addr.arpa. 3600 IN	PTR	ns1.google.com.

        ;; Query time: 36 msec
        ;; SERVER: 127.0.0.53#53(127.0.0.53)
        ;; WHEN: Сб фев 12 18:12:57 MSK 2022
        ;; MSG SIZE  rcvd: 83
