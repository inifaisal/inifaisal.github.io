---
layout: post
section-type: post
title: Buat Websit Gratis dengan Jekyll di Github
description: Jekyll adalah static site generator yang dibuat dengan Ruby
category: Tutorial
tags: [ 'github', 'jekyll', 'blog' ]
---

### Apa sih Jekyll itu?

Jekyll adalah *static site generator* yang pertama kali dirilis pada tahun 2008, dibuat oleh Tom Preston-Waner dengan menggunakan [ruby](https://id.wikipedia.org/wiki/Ruby_(bahasa_pemrograman)). Jekylll bisa merender file dengan format markdown, textile dan file html biasa tentunya, templete engine yang digunakan adalah Liquid. Jekyll merupakan engine yang digunakan oleh github pages dan pihak github membolehkan kita untuk menghost website kita di repository mereka.


### Cara Install Jekyll

Sebelum kita menghosting website kita digithub, sebaiknya kita siapkan dulu tools-tools yang akan kita gunakan:

Pertama cek dulu apakah ruby sudah terinstall di komputer/laptop kalian, dengan mengetikkan perintah berikut diterminal (cmd)

```console
$ ruby -v
```

jika hasilnya seperti

{% highlight console %}
$ ruby x.x.x bla bla bla ..
{% endhighlight %}

berarti ruby sudah terinstall di komputer/laptop kalian, jika hasilnya berbeda, silahkan install dulu ruby di komputer/laptop kalian, caranya untuk pengguna ubuntu, silahkan buka terminal dan ketikkan perintah berikut!

{% highlight console %}
$ sudo apt-get install ruby
{% endhighlight %}

jika sudah terinstall, kita lanjut install jekyll, masih di terminal, ketikkan perintah berikut!

{% highlight console %}
$ gem install jekyll
{% endhighlight %}

setelah itu, saatnya memulai membuat website kita, ketikkan perintah berikut pada terminal kalian!

{% highlight bash %}
$ jekyll new nama-blog-kalian
{% endhighlight %}

dan cd ke directori "nama-blog-kalian", karena Jekyll sudah disertakan webserver maka kalian dapat melihat website kalian secara local, untuk melakukan hal tersebut, silahkan ketikkan perintah berikut pada terminal!

{% highlight bash %}
$ jekyll serve
{% endhighlight %}

dan buka browser favorite kalian, masukkan alamat 127.0.0.1:4000, maka website kalian pun telah jadi. Saatnya kita mengupload website kalian tadi ke repositori github, caranya adalah sebagai berikut:

- Buat dulu [repository baru di github](https://github.com/new), namakan dengan "username-kalian.github.io"

![menamakan repositori baru di github]({{ site.baseurl }}/img/menamakan-repository-baru-di-github.png)

pilihan "*Initialize this repository with a README*" jangan di centang!

- Pada terminal ketikkan perintah berikut!

{% highlight bash %}
$ git init
$ git add --all
$ git commit -m "First commit"
$ git remote add origin remote repository https://github.com/xxx/xxx.github.io
$ git push origin master
{% endhighlight %}

Jika semuanya sudah benar dan berjalan lancar, silahkan buka xxx.github.io pada browser dan horeee website kalian telah online.

note: ganti xxx dengan username github kalian

Sekian terima kasih!