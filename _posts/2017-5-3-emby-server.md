---
layout: post
title: آموزش راه اندازی مدیا سرور Emby
category: آموزشی
---
![تصویری از مدیا سرور]({{ site.baseurl }}/images/post/emby-server.png "Emby Server")
چند وقتی بود که دوست داشتم فیلم هایی که داخل کامپیوتر خودم دارم رو بتونم بدون استفاده از فلش مموری داخل پخش کننده خانگی ببینم … این پخش کننده ما امکاناتی مثل FTP یا Kodi نداشت اما وای فای داشت که DLNA هم پشتیبانی میکرد برای همین به فکر افتادم تا فیلم هایم را با استفاده از DLNA روی شبکه به اشتراک بزارم و برای اینکار برنامه ی Emby رو پیدا کردم …

برای نصب Emby Server در توزیع های گنو لینوکس:

```
https://software.opensuse.org/download.html?project=home%3Aemby&package=emby-server
```

پس از نصب با استفاده از دستورات زیر سرور را اجرا کرده :

```shell
$ sudo systemctl start emby-server
$ sudo systemctl enable emby-server
```

 حال که Emby Server اجرا شد از طریق لینک زیر می توان به آن دسترسی داشت:

```
http://localhost:8090
```

 وقتی برای اولین بار وارد تنظیمات سرور شدید یک ویزارد برای شما باز شده و تنظیمات آنرا انجام میدهید (تنظیمات سختی نداشت اما زمان انجام یادم رفت عکس بگیرم 😐  ).

اما کل کاری که باید انجام بدید به این صورت هست که فولدری که ویدئو های شما در اون قرار داره باید به سرور معرفی بشه.

حالا وقتی دستگاه پخش کننده شما به وای فای وصل باشه و وارد برنامه ی  DLNA DMP شوید فولدری که به اشتراک گذاشته اید را مشاهده کرده و میتوانید تمامی ویدئو هایتان را به راحتی مشاهده کنید. 😉