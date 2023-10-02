# HTTP HTTPS и их параметры\
_________________________________________________________________________
## Лабораторная работа №1
### Куриленко М.О. АСБ-3-036
Команда для HTTP запросов: curl -l -v example.ru 
_________________________________________________________________________
### RGUPS
processing: www.rgups.ru
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 80.72.224.90:80...
* Connected to www.rgups.ru (80.72.224.90) port 80
> GET / HTTP/1.1
> Host: www.rgups.ru
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 301 Moved Permanently
< Server: nginx/1.19.1
< Date: Fri, 29 Sep 2023 06:38:40 GMT
< Content-Type: text/html
< Content-Length: 169
< Connection: keep-alive
< Location: https://www.rgups.ru/
<
{ [169 bytes data]
100   169  100   169    0     0    716      0 --:--:-- --:--:-- --:--:--   722<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>nginx/1.19.1</center>
</body>
</html>

* Connection #0 to host www.rgups.ru left intact
_________________________________________________________________________
### GitHub
* processing: github.com
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 140.82.121.3:80...
* Connected to github.com (140.82.121.3) port 80
> GET / HTTP/1.1
> Host: github.com
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 301 Moved Permanently
< Content-Length: 0
< Location: https://github.com/
<
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
* Connection #0 to host github.com left intact
_________________________________________________________________________
###