---
layout: post
section-type: post
title: Cara Install Node.js di Windows, Linux dan Mac OS dengan Mudah
category: Tutorial
tags: [ 'javascript', 'nodejs' ]
---

Pada tutorial kali ini saya akan memberikan cara mudah untuk mengintall node.js di Windows, Linux dan Mac OS.

![Node.js Logo](/img/nodejs-logo.png)

### Apa itu Nodejs

Node.js adalah platform perangkat lunak pada sisi-server dan aplikasi jaringan. Ditulis dengan bahasa javascript dan bisa dijalankan pada Windows, Mac OS X dan Linux tanpa perubahan kode program. Node.js memiliki pustaka server HTTP sendiri sehingga memungkinkan untuk menjalankan webserver tanpa menggunakan program webserver seperti Apache atau nginx.

Node.js dibuat oleh Ryan Dahl pada tahun 2009, menggunakan teknologi v8 javascript engine yang di gunakan oleh google chrome, pada node.js telah di lengkapi paket manager yaitu NPM (node package manager).


### Cara Install Node.js di Windows
Cara install node.js di windows sangatlah mudah sama seperti mengintall aplikasi kebanyakan cukup, klik next, next dan next hingga selesai, tapi sebelumnya kalian harun mengunduh dulu file instalasinya di [website resmi node.js](https://nodejs.org/en/download/).


### Cara Install Node.js di Linux
Untuk di Linux ada berbagai cara namun kesemua cara tersebut hampir sama, pada tutorial ini saya hanya memberikan cara menginstall node.js di linux Debian based, yaitu Ubuntu dan turunannya seperti Linux Mint dan Elementery Os, untuk Distro linux yang lain silahkan kalian merujuk pada [website resmi node.js](https://nodejs.org/en/download/package-manager/). baiklah langsung saja cara install node.js di linux, pada terminal jalankan perintah berikut!

``` bash
$ curl -sL https://deb.nodesource.com/setup_4.x | sudo -E bash -
$ sudo apt-get install -y nodejs
```


### Cara Install Node.js di Mac Os
Pada Mac Os cara install node.js sangatlah mudah, hampir sama dengan cara menginstall node.js di windows, yang berbeda hanya file instalasinya saja, tentunya kalian harus mengunduhnya dulu di [website resmi node.js](https://nodejs.org/en/download/).


### Cara Mengganti Versi Node.js Tanpa Install Ulang dengan [n (Node version management)](https://github.com/tj/n)
Adakalanya kita ingin mengupdate versi nodejs ke versi paling terbaru namun takut ada beberapa module yang belum cocok dengan versi terbaru dari node.js tersebut, nah daripada repot-repot install ulang, lebih baik kalian menggunakan n, cara install n sangatlah mudah, pada terminal jalankan perintah berikut!

``` bash
$ sudo npm install -g n
```

Setelah n terinstall dan kalian ingin untuk mengganti versi node.js yang kalian gunakan cukup dengen menjalankan perintah berikut pada terminal!

``` bash
$ n latest
# untuk mengintall versi terbaru
$ n stable
# untuk mengintall versi stabil
$ n 4.2.4
# untuk mengintall versi tertentu
```

Note: untuk kalian pengguna os windows, n belum bisa di gunakan pada os kalian :disappointed:.
Selamat kalian telah berhasil menginstall Node.js di Komputer/Laptop kalian :clap:.