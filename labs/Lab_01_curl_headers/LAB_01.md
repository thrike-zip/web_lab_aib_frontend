# HTTP HTTPS и их параметры
_________________________________________________________________________
## Лабораторная работа №1
### Куриленко М.О. АСБ-3-036
-I - указывает отправить только заголовки HTTP-ответа сервера, без тела ответа.
-v - делает подробный вывод информации о запросе.
-L - указывает следовать перенаправлениям при запросе, если сервер возвращает код (301 или 302).
Команда для HTTP запросов: curl -l -L -v example.ru 
_________________________________________________________________________
### RGUPS
* processing: rgups.ru
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 80.72.224.90:80...
* Connected to rgups.ru (80.72.224.90) port 80
> GET / HTTP/1.1
> Host: rgups.ru
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 301 Moved Permanently
< Server: nginx/1.19.1
< Date: Thu, 30 Nov 2023 06:25:04 GMT
< Content-Type: text/html
< Content-Length: 169
< Connection: keep-alive
< Location: https://rgups.ru/
<
{ [169 bytes data]
100   169  100   169    0     0    939      0 --:--:-- --:--:-- --:--:--   949<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>nginx/1.19.1</center>
</body>
</html>

* Connection #0 to host rgups.ru left intact 
_________________________________________________________________________
### GitHub
* processing: github.com
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 140.82.121.4:80...
* Connected to github.com (140.82.121.4) port 80
> GET / HTTP/1.1
> Host: github.com
> User-Agent: curl/8.2.1
> Accept: */*
>
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0< HTTP/1.1 301 Moved Permanently
< Content-Length: 0
< Location: https://github.com/
<
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
* Connection #0 to host github.com left intact

_________________________________________________________________________
###🚝 РЖД
* processing: rzd.ru
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 212.164.138.126:80...
* Connected to rzd.ru (212.164.138.126) port 80
> GET / HTTP/1.1
> Host: rzd.ru
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 301 Moved Permanently
< Date: Thu, 30 Nov 2023 06:25:42 GMT
< Content-Type: text/html
< Content-Length: 150
< Connection: keep-alive
< Location: https://rzd.ru:443/
<
{ [150 bytes data]
100   150  100   150    0     0    567      0 --:--:-- --:--:-- --:--:--   570<html>
<head><title>301 Moved Permanently</title></head>
<body bgcolor="white">
<center><h1>301 Moved Permanently</h1></center>
</body>
</html>

* Connection #0 to host rzd.ru left intact

_________________________________________________________________________
###🕸 Яндекс
* processing: yandex.ru
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 5.255.255.77:80...
* Connected to yandex.ru (5.255.255.77) port 80
> GET / HTTP/1.1
> Host: yandex.ru
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 302 Moved temporarily
< Accept-CH: Sec-CH-UA-Platform-Version, Sec-CH-UA-Mobile, Sec-CH-UA-Model, Sec-CH-UA, Sec-CH-UA-Full-Version-List, Sec-CH-UA-WoW64, Sec-CH-UA-Arch, Sec-CH-UA-Bitness, Sec-CH-UA-Platform, Sec-CH-UA-Full-Version, Viewport-Width, DPR, Device-Memory, RTT, Downlink, ECT
< Cache-Control: max-age=1209600,private
< Date: Thu, 30 Nov 2023 06:26:18 GMT
< Location: https://dzen.ru/?yredirect=true
< NEL: {"report_to": "network-errors", "max_age": 100, "success_fraction": 0.001, "failure_fraction": 0.1}
< P3P: policyref="/w3c/p3p.xml", CP="NON DSP ADM DEV PSD IVDo OUR IND STP PHY PRE NAV UNI"
< Portal: Home
< Report-To: { "group": "network-errors", "max_age": 100, "endpoints": [{"url": "https://dr.yandex.net/nel", "priority": 1}, {"url": "https://dr2.yandex.net/nel", "priority": 2}]}
< Transfer-Encoding: chunked
< X-Content-Type-Options: nosniff
< X-Robots-Tag: unavailable_after: 12 Sep 2022 00:00:00 PST
< X-Yandex-Req-Id: 1701325578105081-6282373200047179565-balancer-l7leveler-kubr-yp-vla-88-BAL-8843
< set-cookie: is_gdpr=0; Path=/; Domain=.yandex.ru; Expires=Sat, 29 Nov 2025 06:26:18 GMT
< set-cookie: is_gdpr_b=CIfNMhDh3AEoAg==; Path=/; Domain=.yandex.ru; Expires=Sat, 29 Nov 2025 06:26:18 GMT
< set-cookie: _yasc=MiLVhhtNCQp7ylqjz4Sb3AhO7YHUaDoUhGsDUlQOe8KpJiAFbqOL8EBs+NZTqoof93sU; domain=.yandex.ru; path=/; expires=Sun, 27 Nov 2033 06:26:18 GMT; secure
<
{ [5 bytes data]
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
* Connection #0 to host yandex.ru left intact

_________________________________________________________________________
###🐍 Python
* processing: python.org
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 151.101.128.223:80...
* Connected to python.org (151.101.128.223) port 80
> GET / HTTP/1.1
> Host: python.org
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 301 Moved Permanently
< Connection: close
< Content-Length: 0
< Server: Varnish
< Retry-After: 0
< Accept-Ranges: bytes
< Date: Thu, 30 Nov 2023 06:26:51 GMT
< Via: 1.1 varnish
< X-Served-By: cache-fra-eddf8230127-FRA
< X-Cache: HIT
< X-Cache-Hits: 0
< X-Timer: S1701325612.741800,VS0,VE0
< Location: https://www.python.org/
< Strict-Transport-Security: max-age=315360000; preload
<
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
* Closing connection

_________________________________________________________________________
###🌠 Saint GIT
* processing: git-scm.com
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 188.114.98.234:80...
* Connected to git-scm.com (188.114.98.234) port 80
> GET / HTTP/1.1
> Host: git-scm.com
> User-Agent: curl/8.2.1
> Accept: */*
>
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0< HTTP/1.1 301 Moved Permanently
< Date: Thu, 30 Nov 2023 06:27:23 GMT
< Transfer-Encoding: chunked
< Connection: keep-alive
< Cache-Control: max-age=3600
< Expires: Thu, 30 Nov 2023 07:27:23 GMT
< Location: https://git-scm.com/
< Server: cloudflare
< CF-RAY: 82e106358eaa380e-FRA
<
{ [5 bytes data]
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
* Connection #0 to host git-scm.com left intact
_________________________________________________________________________
###🐵 Jetbrains
* processing: jetbrains.com
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 18.66.112.6:80...
* Connected to jetbrains.com (18.66.112.6) port 80
> GET / HTTP/1.1
> Host: jetbrains.com
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 301 Moved Permanently
< Server: CloudFront
< Date: Thu, 30 Nov 2023 06:27:51 GMT
< Content-Type: text/html
< Content-Length: 167
< Connection: keep-alive
< Location: https://jetbrains.com/
< X-Cache: Redirect from cloudfront
< Via: 1.1 f952757fdddf3c9caa357164f2d464d8.cloudfront.net (CloudFront)
< X-Amz-Cf-Pop: FRA56-P5
< Alt-Svc: h3=":443"; ma=86400
< X-Amz-Cf-Id: 7OredPffA_B-NLwVPzb3TVVQb9FLSMKZxfwnkT6Vd1CdQW7cwBy1VQ==
<
{ [167 bytes data]
100   167  100   167    0     0    452      0 --:--:-- --:--:-- --:--:--   453<html>
<head><title>301 Moved Permanently</title></head>
<body>
<center><h1>301 Moved Permanently</h1></center>
<hr><center>CloudFront</center>
</body>
</html>

* Connection #0 to host jetbrains.com left intact

_________________________________________________________________________
###💪 VSC
* processing: code.visualstudio.com
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0*   Trying 13.107.246.45:80...
* Connected to code.visualstudio.com (13.107.246.45) port 80
> GET / HTTP/1.1
> Host: code.visualstudio.com
> User-Agent: curl/8.2.1
> Accept: */*
>
< HTTP/1.1 307 Temporary Redirect
< Date: Thu, 30 Nov 2023 06:28:19 GMT
< Content-Type: text/html
< Content-Length: 0
< Connection: keep-alive
< Location: https://code.visualstudio.com/
< x-azure-ref: 20231130T062819Z-xbw71y738t64128u3m4vnx2n5w00000002ug00000000u5eg
< X-Cache: CONFIG_NOCACHE
<
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
* Connection #0 to host code.visualstudio.com left intact
_________________________________________________________________________