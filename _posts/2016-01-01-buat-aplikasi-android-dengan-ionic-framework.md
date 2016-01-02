---
layout: post
section-type: post
title: Buat Aplikasi Android dengan Ionic Framework
category: Mobile
tags: [ 'android', 'ionic' ]
---

Hai, Pada postingan kali ini saya akan memberikan tutorial sederhana bagaimana caranya membuat aplikasi android dengan mengunakan ionic framework.

![Ionic Logo](/img/ionic_logo-173x192.png)

### Apa itu Ionic Framework?
[Ionic](https://ionicframework.com) Framework adalah sebuah framework yang dibuat dengan menggunakan teknologi HTML5 dengan [AngularJS](https://angularjs.org), ionic sangat mudah di pelajari dan juga mempunyai tampilan yang hampir mirip dengan aplikasi android native.

### Kenapa Ionic?
Berikut ini beberapa kelebihan Ionic di bandingankan dengan framework sejenis:

- Performanya mantap
- Tampilannya hampir mirip dengan Aplikasi Native
- Designnya yang keren
- Banyak Pluginnya
- Dilengkapi dengan fitur CLI yang Powerfull, dan
- Mudah untuk dipelajari


### Cara Install Ionic
Syarat utama sebelum kalian memulai membuat aplikasi berbasis ionic adalah pada Kamputer/Laptop kalian harus sudah terinstall Java JDK, [Android SDK](https://developer.android.com/sdk/) dan [Nodejs](https://nodejs.org), kalau belum silahkan install dulu, karena saya tidak akan menjelaskan cara menginstall ketika tools tersebut pada tutorial ini, yang akan saya jelaskan disini adalah cara install ionic, baiklah langsung saja, cara install ionic itu adalah sebagai berikut:

- Pertama install dulu Cordova, dengan mengetikkan perintah berikut di terminal pada linux atau CMD untuk windows!

``` bash
$ npm install -g cordova
```

- Setalah Cordova terinstall saatnya install ionic

``` bash
$ npm install -g ionic
```

Jika semuanya berjalan lancar, saatnya kita membuat aplikasi android.

### Membuat Aplikasi Sederhana dengan Ionic

Pada Terminal/CMD ketikkan perintah berikut!

``` bash
$ ionic start nama-aplikasi-kalian
```

Setelah itu masuk ke folder aplikasi yang baru saja kalian buat dan ketikkan perintah berikut pada terminal/CMD!

``` bash
$ ionic add platform android
```

Setelah itu saatnya mencoba aplikasi yang baru saja kalian buat pada perangkat Android kalian, ketikkan perintah berikut pada terminal/CMD!

``` bash
$ ionic run
```

jika semuanya berjalan lancar, lihat pada perangkat Android kalian dan Hooooree aplikasi android kalian pun telah selesai :smile:

Pada postingan berikutnya saya akan memberikan tutorial cara membuat aplikasi CRUD sederhana di Android dengan menggunakan ionic tentunya, so stay tune ya!

Sekian Terima Kasih.
