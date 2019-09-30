---
layout: post
title: "Hello World Again"
description: "Memulai sesuatu yang baru kembali"
date: 2019-05-26
categories: [articles]
tags: [introduction, welcoming]
comments: true
share: true
hidden: false
---

Hello World *Again*. Akhirnya dapat memulai kembali kegiatan menulis.

Setelah melewati kesibukan-kesibukan lain didunia nyata dan ditengah [sabatical leave](blog/sabatical-leave/) yang sedang dijalani (walaupun tidak seperti [sabatical leave pada umumnya](https://www.thebalancecareers.com/why-employers-should-consider-sabbatical-leave-programs-4171929)), akhirnya dapat kembali menulis dan menjalani kebiasan lama untuk nge-blog. Kemudian saya menyadari bahwa blog ini ([harapan.me](https://www.harapan.me)) sudah lama tidak diurus serta tidak banyak tulisan yang dipublish selama 6 bulan terakhir dan blog lama ([notes.rioharapan.com](http://notes.rioharapan.com)) yang akhirnya mati dengan terpaksa. Dalam hal desain front-end dan tampilannya juga tidak banyak berubah sejak awal dibuat yaitu di April 2017 hingga terakhir kali update pada Desember 2018.

Untuk memulai kembali blog ini sebelum menerbitkan tulisan-tulisan terbaru, harus diperlukan suatu tampilan baru, bentuk baru dan konsep baru (tampilan lama dan blog lama bisa diakses di-[v01](https://www.harapan.me)). Maka kemudian terbentuklah tampilan blog ini yang lebih sederhana dan agak sedikit fluid dari versi sebelumnya. Akhirnya selesailah desain blognya seperti ini. Dari sisi teknologi, tetap teknologi dibelakang blog ini menggunakan jekyll, markdown dan dihosting di-github.io, dengan domain tetap menggunakan [harapan.me](https://www.harapan.me). Lalu karena Google Chrome pada update-an terbarunya akan [melabeli website yang tidak menggunakan https sebagai website yang tidak aman](https://security.googleblog.com/2018/02/a-secure-web-is-here-to-stay.html), terpaksalah website ini harus dipasangi ssl, walaupun memang tidak ada data credentials yang dipertukarkan diblog ini. Saya akhirnya memindahkan management domain ini dengan menggunakan [cloudfare](https://www.cloudflare.com/) agar mendapatkan [certificate https secara gratis](https://www.cloudflare.com/ssl/). Akhirnya terbentuklah blog ini, dengan biaya hanya US$ 14.15 yang hanya digunakan untuk membeli domain di-[namesilo](https://www.namesilo.com/pricing.php?rid=43f3493rl). Mengenai stack technology dari blog ini, penjelasan lebih rincinya dapat dilihat dihalaman berikut [Bagaimana harapan.me dibentuk secara teknologi?](/blog/tech-stack-harapan-me/)

Secara umum saya banyak terinspirasi dari beberapa orang dalam bidang teknologi yang begitu rajin menulis dan membagikan tulisannya secara konsisten. Orang tersebut salah satunya ialah [Joel Spolsky](https://en.wikipedia.org/wiki/Joel_Spolsky) seorang software engineer, founder [stackoverflow.com](https://stackoverflow.com/) dan [trello](https://trello.com/). Dia telah memulai blogging sejak tahun 1999 dengan alamat blog di-[joelonsoftware](https://www.joelonsoftware.com). Dalam blognya Joel banyak menulis dari hal-hal teknis menyangkut dunia programming hingga architecture software, management, product design hingga pengalaman pribadinya. Beberapa articlenya menjadi sangat terkenal hingga menjadi referensi informal bagi orang-orang, seperti [Things You Should Never Do, Part I](https://www.joelonsoftware.com/2000/04/06/things-you-should-never-do-part-i/) dan [How Microsoft lost the api war](https://www.joelonsoftware.com/2004/06/13/how-microsoft-lost-the-api-war/).

Pengalaman yang panjang dan dengan tulisan yang hampir mencapai 1100 artikel dengan berbagai topik serta konsistensi yang tinggi membuat blog-nya cukup terkenal dan memilki tema dan konsep yang kuat. Joel pada tulisannya berfokus pada profesional karir yang dihadapinya sebagai software engineer hingga sekarang sebagai CEO [Stackexchange](https://stackexchange.com/). Oleh karena itu saya juga berpikir untuk mengambil satu tema pada blog ini. Karena secara profesional saya berkecimpung didunia data dan cloud, maka tema blog ini akan banyak menitik beratkan kepada dua topik tersebut dengan mungkin beberapa artikel ringan dan beberapa review tentang buku yang telah saya baca serta pengalaman-pengalaman yang cukup menarik untuk dibagikan. Silahkan baca artikel berikut [archiavelli](blog/archiavelli/) untuk asal nama, tema, bentuk penulisan dan fokus blog ini.

Akhir kata, saya mengucapkan selamat membaca, semoga hal-hal yang ada disini dapat berguna. Silahkan tinggalkan pesan dan mari berinteraksi. 

```python
def print_hello(reader):
	print("Hello " + str(reader))
	print("Selamat Membaca!")

if __name__ == '__main__':
	print_hello('<your-name>')
```

