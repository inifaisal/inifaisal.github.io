---
layout: post
section-type: post
title: Cara Buat Aplikasi Angular 2 dengan Webpack
category: Tutorial
tags: [ 'angular2', 'javascript' ]
---

Dalam pengembangan aplikasi berbasis angular 2 itu ada berbagai cara yang bisa ditempuh, karena aplikasi yang akan kita buat nantinya berbasis es6 yang mana pada saat ini belum banyak didukung oleh kebanyakan browser pengguna, maka dari itu kita membutuhkan sebuah module yang digunakan untuk mengubah aplikasi yang kita buat memjadi berbasis es5, salah satu module tersebut adalah [webpack](https://github.com/webpack/webpack). Pada pengembangan aplikasi ini kita tidak menggunakan javascript melainkan yang kita gunakan adalah [typescript](https://typescriptlang.org), kenapa typescript? karena selain sesuai dengan anjuran dari pengembang angular itu sendiri, alasan utama kenapa kita mengunakan typescript adalah kerena mudah dalam memahami dan mempelajari sintax-sintaxnya serta lebih mudah dibaca jika di bandingkan dengan vanila javascript (menurut pendapat saya pribadi :smile:), kok bisa? silahkan saja anda buktikan sendiri setelah mempelajari tutorial ini, silahkan bandingkan.

### Persiapan
Sebelumnya install dulu beberapa module berikut ini secara global di system kalian, dengan menjalankan perintah berikut di terminal!

{% highlight bash %}
$ sudo npm install typescript tds
{% endhighlight %}

Setelah terinstall, silahkan anda unduh atau clone dulu repository berikut [angular2-minimal-starter](https://github.com/inifaisal/angular2-minimal-starter), setelah itu, cd atau masuk ke directory angular2-minimal-starter dan pada terminal jalankan perintah berikut!

{% highlight bash %}
$ npm install
{% endhighlight %}
Berikutnya jalankan pula perintah berikut!

{% highlight bash %}
$ tds install
{% endhighlight %}

Perintah diatas akan menginstall semua module-module yanng kita butuhkan, sampai tahap ini aplikasi kita sudah bisa di jalankan namun belum menampilkan apa-apa, saatnya ketahapan berikutnya.

### Hello world
setelah semua module terinstall, saatnya kita membuat aplikasi sederhana yaitu menampilkan tulisan "Hello World" pada browser.

- di folder src/app ada file app.ts, buka dan edit file tersebut dengan menggunakan text editor favorite kalian, edit agar sesuai dengan script berikut!

{% highlight javascript %}
import {Componen} from 'angular2/core';

@Componen({
	selector: 'main-app',
	template: `
		<h1>Hello world</h1>
		`
})

export class App{

}
{% endhighlight %}

- Setelah itu pada folder src ada file bootstrap.ts, buka dan edit file tersebut, seperti pada script berikut!

{% highlight javascript %}
import {bootstrap} from 'angular2/platform/browser';


import {App} from './app/app';

document.addEventListener('DOMContentLoaded', function main() {
	bootstrap(App)
		.catch(err => console.error(err));
});
{% endhighlight %}

- Selanjutnya pada folder src/public, buat sebuat file index.html dan masukkan script berikut!

{% highlight html %}
<!DOCTYPE html>
<html lang="en">
<head>
  <title>Angular2 Minimal Starter</title>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">
</head>
<body>

  <main-app>
    Loading...
  </main-app>

  <!-- Common files to be cached -->
  <script src="/__build__/common.js"></script>
  <!-- Vendor files -->
  <script src="/__build__/vendor.js"></script>
  <!-- App script -->
  <script src="/__build__/app.js"></script>
</body>
</html>
{% endhighlight %}

- Setelah itu saatnya menjalankan aplikasi yang telah kita buat tersebut, jalankan perintah berikut pada terminal!

{% highlight bash %}
$ npm run server
{% endhighlight %}

Jika tak ada yang error, seperti yang terlihat pada gambar berikut:

![angular 2](/img/run-angular-2-webpack.png)

silahkan buka browser dan masukkan alamat 127.0.0.1:3000 dan pastikan anda melihat tulisan Hello world, seperti yang terlihat pada gambar berikut:

![angular 2](/img/success-run-angular2.png)

Dan aplikasi sederhana kita pun telah jadi, selanjutnya terserah anda, silahkan anda kembangkan sendiri aplikasi tersebut :smile:

Jika anda mempunyai pertanyaan atau ada yang kurang di mengerti, silahkan anda bertanya pada kolom komentar di bawah!


### Daftar Bacaan
- [Dokumentasi Angular 2](https://angular.io/docs)
- [Dokumentasi TypeScript](https://github.com/Microsoft/TypeScript/wiki)
- [Dokumentasi Webpack](https://webpack.github.io/docs)
- [Kumpulan Tutorial Komprehensif tentang Angular 2](http://blog.thoughtram.io/exploring-angular-2)
- [Kumpulan Tutorial Lainnya tentang Angular 2](http://onehungrymind.com)

Sekian terima kasih, semoga bermanfaat.
