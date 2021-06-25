---
layout: post
title: "Implementing Big Data Engineering For Business in The Modern Era"
description: "Tech Talk yang merupakan bagian dari Glints Expert Class ini membahas mengenai pengalaman dalam mengimplementasikan Big Data untuk membuat dampak pada perkembangan Bisnis diperusahaan"
date: 2021-06-11
categories: 'talks'
inreview: false
tags: [talks, bigdata, glints]
permalink: /bigdata-glints
comments: true
share: true
hidden: true
---

Jumat ini, 11 Juni 2021, saya berkesempatan untuk mengisi salah satu [Event Expert Class](https://glints.com/id/expert-class) yang diselenggarakan oleh [Glints](https://glints.com/id). Glints Expert Class sendiri merupakan suatu Event yang rutin diadakan oleh Glints, sebuah Talent Platform Career Development di Asia Tenggara. Expert Class ini akan menghadirkan seorang professional disuatu bidang untuk sharing tentang pengalaman mereka, salah satu series yang ada yaitu [Data and Analytics Series](https://glints.com/id/expert-class?categories=Data+%26+Analytics). Dalam Data and Analytics Series ini saya membawakan Topik mengenai Implementasi Big Data.

Materi yang saya bawakan bisa dilihat pada slide berikut,

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vRK7HxS01eQOrJNpUBt5lViJ8z3taVqkceKimnquh-r-A5k96M4JxKWLOmObCIWuPL_q8GltQzEOZLw/embed?start=false&loop=false&delayms=3000" frameborder="0" width="820" height="496" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

<br >
Dalam menyusun materi ini sebelumnya, saya menuliskannya terlebih dahulu outline-nya, lalu kemudian mencoba menarasikannya seraya membuat materinya di-slides. Dengan sedikit editing sana-sini dan perbaikan, hasil narasinya saya coba post diblog ini.

### Introduction

Dalam Talks kali ini, saya akan menyampaikan dan sharing sedikit tentang pengalaman yang pernah saya lalui dalam mengimplementasikan Big Data Platform dibeberapa perusahaan tempat saya bekerja sebelumnya. Namun sebelum kita berbicara lebih jauh, alangkah baiknya untuk kita berkenalan terlebih dahulu.

Saya, Rio Harapan Pangihutan. Sejak 2019 saya bekerja di-[LinkAja](https://www.linkaja.id/) sebagai Data Engineer Specialist/Principal, nanti dibagian selanjutnya saya akan banyak membahas pengalaman saya di-LinkAja dalam membangun Big Data Platform . Sebelumnya saya sempat bekerja sebagai Data Science Consultant di-[Stream Intelligence](http://streamintelligence.com/) untuk membantu salah satu Retail Company dalam mengimplementasikan Data Platform untuk mendukung Marketing Analytics yang mereka lakukan. Sejak tahun 2017 hingga 2019 saya bekerja di-beberapa perusahaan dan projects sebagai data engineer. Diluar pekerjaan saya melakukan hobby saya yaitu Hiking dan Diving. Terutama ketika weekend dan libur panjang, saya akan melakukan [hiking ke gunung](/thesummits) yang bisa dijelajahi dalam waktu 2 atau 3 hari. Selain itu, saya juga melakukan diving dan merupakan [diver yang tersertifikasi](/diver). Mungkin, beberapa hal tersebut yang bisa saya ceritakan dalam perkenalan kali ini.

### Let's Talk about Big Data

Topik bahasan kita kali ini, akan coba kita bagi dalam 3 bagian. Bagian pertama berjudul __"What?"__ Dibagian ini kita akan coba lihat dulu, tentang Big Data itu, apa sih Big Data tersebut dan apa sebenarnya permasalahan yang bisa diselesaikan dengan Big Data ini? Selanjutnya bagian kedua berjudul __"Implementing"__, 
Bagian terakhir dari topik kita kali ini berjudul __"Be Prepared"__, dibagian ini kita akan membahas mengenai langkah praktis yang bisa kita lakukan untuk mempersiapkan diri kita, jika nanti suatu saat kita terlibat dalam satu project untuk mengimplementasikan Big Data. 

### Big Data. What? The Problem?

Big Data mulai banyak dibicarakan akhir-akhir ini, menjadi populer dan trending dalam pembicaraan tentang teknologi di-internet. Big data menjadi jargon dan tren baru, karena akan diprediksi untuk menghadirkan suatu terobosan baru yang dapat membantu perkembangan bisnis. Namun apasih sebenarnya Big Data itu? Sebelum membahas mengenai Big Data, mari kita kupas terlebih dahulu darimana tren ini muncul.

Semua ini berasal dari sebuah kata yang diucapkan oleh Tokoh Management terkenal abad 20, yaitu Peter Drucker dan W. Edwards Deming.

> “You can’t manage what you don’t measure.”

Prinsip yang disebarkan mereka dalam mengajar tentang management tersebut membuat perubahan besar dalam management dibanyak perusahaan. Dengan mengukur dan mengolah data yang ada, para manager dapat mengukur performa bisni mereka. Tidak hanya itu, mereka juga dapat mengetahu pengetahuan baru mengenai pelanggan, bisnis dan banyak hal lainnya. Kemudian menggunakan pengetahuan tersebut untuk meningkatkan performa mereka dan mengambil keputusan<sup>[1](#reference)<sup>.

Dalam sejarahnya juga, perkembangan teknologi membuat penyimpanan data dan pemrosesan data semakin murah<sup>[3](#reference)</sup>. Hal ini akan berimplikasi langsung terhadap pertumbuhan data yang disimpan. Kita bisa melihat dalam gambar pada slide ketujuh<sup>[2](#reference)</sup>. Pada sekitar tahun 1980-2000an, penyimpanan data masih dalam bentuk penyimpanan analog, seperti dalam fonograf, kaset dan buku-buku. Sebelum tahun 1993, semua data masih disimpan dalam format analog. Hingga kemunculan Floppy Disk, CD dan media penyimpanan digital lainnya membuat perubahan bentuk penyimpanan menjadi dalam bentuk digital. Pada tahun 2007 berdasarkan data yang dikutip dari beberapa sumber<sup>[4](#reference)</sup> menunjukkan perbandingan penggunaan antara data digital dan data analog begitu jomplang. Jumlah data digital yang tersimpan diperkirakan mencapai 280 Exabytes, sedangkan data analog hanya sekitar 19 Exabytes (1 Exabytes = 1,000,000 Terrabytes).

Data-data yang disimpan tidak hanya sekedar data yang berasal dari transaksi, perusahaan mencoba untuk mengukur setiap metrik yang ada dan menyimpannya, untuk kemudian dapat diolah dan menghasilkan suatu wawasan dan pengetahuan baru tentang bisnis mereka. Contoh kasus yang paling terkenal ialah kebangkitan Amazon sebagai perusahaan toko buku online yang bisa menyingkirkan banyak toko buku tradisional offline dengan mengutilisasi data dengan benar.

Amazon berusaha untuk merekam setiap transaksi, program loyalti, buku yang dibeli setiap konsumen, buku yang dilihat oleh konsumen, perilaku konsumen dalam memilih buku dan banyak data lainnya, mereka merekam setiap individu konsumen. Data yang mereka punya berlimpah ruah (big data). Dengan menggunakan data tersebut mereka dapat membuat algoritma untuk memberikan rekomendasi kepengguna, lalu membuat pengguna merasa nyaman dengan layout, mengukur seberapa bagus metode promosi yang diberikan kepada setiap individu diwebsite mereka serta banyak hal yang tidak dapat dilakukan toko buku offline lainnya.

Amazon dapat melakukan bisnis dengan cara baru. Perubahan terjadi dalam mereka berbisnis dan cara kerja mereka sehingga menghasilkan banyak peluang yang dapat memenangkan mereka dibandingkan perusahaan tradisional. Amazon dapat memperlakukan setiap konsumen mereka secara spesial berdasarkan apa yang mereka ketahui tentang pengguna tersebut dari data yang telah mereka kumpulkan. Dengan data yang besar tersebut, kita dapat mengukur serta pengelolaan kita terhadap bisnis menjadi lebih presisi dari sebelumnya, prediksi dan pengambilan keputusan menjadi lebih tepat. Hal-hal yang dulu ditentukan berdasarkan intuisi yang dibangun selama bertahun-tahun, kini dapat dipelajari dari data.

Berdasarkan kisah sukses dari Amazon tersebut dalam pengimplementasian big data yang mereka lakukan membuat tren baru. Big Data sebagai sebuah filosofi menyebar. Para leader dari berbagai industri melihat big data sebagai sebuah revolusi yang dapat mengubah cara mereka memimpin (terutama dalam pengambilan keputusan yang telah dibahas sebelumnya).

Dalam perkembangan selanjutnya, big data tidak hanya berbicara tentang teknologi atau hal-hal teknis dalam pengelolaan data saja. Seperti yang telah disebutkan sebelumnya bahwa terjadi perubahan dalam keberjalanan bisnis,membuat management dalam perusahaan berubah. Mereka dituntut harus bisa terjun langsung dalam mengurusi hal-hal teknis dalam penggunaan teknologi big data ini. Transisi terjadi. Big Data tidak hanya nama lain untuk menyebut pengolahan data (data analisis).

Ada 5 karakteristik yang membedakan big data dengan data analitik biasa. Karakteristik tersebut dapat dirangkum dalam 5V, yaitu Volume, Velocity, Variety, Veracity dan Value.

#### Volume

V yang pertama ialah Volume yang menyangkut langsung terhadap jumlah data (yang dihasilkan), yaitu Volume. Seperti yang dibahas sebelumnya dengan semakin majunya teknologi penyimpanan data berimplikasi terhadap murahnya harga yang harus dikeluarkan per-giga tempat penyimpanan data, membuat data yang disimpan menjadi semakin banyak. Data bisa dihasilkan dari berbagai sumber, clickstream, history, log, page navigated dan sebagainya. Data yang dihasilkan juga dapat disimpan dalam berbagai format (structured, unstructured dan semi-structured data).

Karena jumlah volume data yang dihasilkan begitu banyak perusahaan yang ingin mengimplementasikan big data harus perangkat (tools) dan metode yang mereka gunakan menyangkut business intelligence dan analitik untuk dapat mengakomodasi bagaimana cara mengumpulkan data dari sistem mereka, menyimpan data, memproses data dan mempresentasikan data.

#### Velocity

V yang kedua ialah Velocity yang menyangkut mengenai kecepatan dari pengumpulan data mereka. Semakin banyaknya pengguna dari produk suatu perusahaan (dalam hal ini seperti web atau aplikasi) semakin banyak data yang dihasilkan. Seandainya setiap kunjungan dari satu pengguna kesebuah website menghasilkan sekitar 10MB data (clickstream, page history, log dan lain sebagainya), bayangkan berapa data yang harus disimpan bila dalam satu hari ada 10 juta pengunjung website tersebut. Data-data tersebut dihasilkan secara masif dan kontinu. Seberapa cepat perusahaan dapat mengumpulan, mengolah data hingga mempresentasikan data tersebut akan berpengaruh terhadap kecepatan mereka membaca pergerakan bisnis dan pengguna hingga kecepatan mereka dalam proses pengambilan keputusan. Tujuan utamanya ialah mencapai waktu yang realtime dalam pengolahan data, dapat dihasilkan informasi yang segera dapat ditampilkan.

#### Variety

V yang selanjutnya ialah Variety. Variety berkolerasi dengan keberagaman data. Data yang dihasilkan bisa dalam berbentuk apa saja, namun pada umumnya dapat dikategorikan menjadi 3, berdasarkan bentuk datanya Structured, Semi-Structured dan Unstructured

_Structured Data_ merupakan data yang sudah terorganisasi, terdefinisi dan tersusun dengan baik, sehingga dapat langsung diproses oleh manusia atau mesin. Contoh structured data ialah data dalam bentuk tabel. Data-data ini sudah tersusun dengan baik mempunyai kolom yang memiliki arti dan bisa direpresentasikan. Structured data dapat dilihat lagi keragamannya berdasarkan data apa yang direpresentasikan oleh masing-masing kolomnya.

_Semi-structured Data_ merupakan data yang bentuknya sudah rapi namun tidak terdefinisi dengan baik. Sebagai contoh log file. Log file sudah rapi dan dapat dibaca dengan baik, namun informasi yang ada didalamnya bisa berbeda-beda antar data, tergantung event yang dicatat oleh log tersebut. Misalnya log file bisa saja berisi timestamp, dan mencatat url yang dikunjungi oleh user, namun dibagian selanjutnya berisi data yang telah diproses oleh server atau error yang dihasilkan oleh sistem. Masing-masing informasi ini butuh pengolahan lebih lanjut untuk mengkategorikannya berdasarkan event-event tertentu dan kemudian dapat direpresentasikan dengan baik.

_Unstructured Data_ bentuk terakhir ialah data yang tidak terorganisasi dan tidak terdefinisi dengan baik sama sekali. Data-data ini biasanya disimpan dalam bentuk file seperti gambar, video, music dan lain sebagainya. Untuk melakukan pengolahan terhadap datanya, kita terlebih dahulu harus merepresentasikan data tersebut dalam bentuk lain seperti misalnya merepresentasikan file gambar menjadi matriks-matriks warna.

Teknologi yang diimplementasikan serta orang-orang yang menggunakannya harus mampu mentranslasikan berbagai jenis data yang beranekaragam untuk dapat menghasilkan informasi yang berguna.

#### Veracity

V yang keempat dalam karakteristik big data ialah Veracity, berhubungan dengan kualitas dan kredibilitas dari data. Data yang dihasilkan begitu banyak, begitu cepat mengalirnya dan begitu beragam, menuntut implementasi teknologi yang dapat menjaga kualitas dan kredibilitas dari data tersebut. Data yang dihasilkan bisa datang dari mana saja sumbernya dan apa saja bentuknya. Ada kemungkinan terjadi kesalahan ketika proses pengumpulan data tersebut terjadi atau terjadinya kesalahan dalam proses transformasi data. 

### Reference

[1. Big Data: The Management Revolution by Andrew McAfee and Erik Brynjolfsson](https://hbr.org/2012/10/big-data-the-management-revolution)

[2. Big Data](https://en.wikipedia.org/wiki/Big_data)

[3. Hard Drive Cost per-Gigabyte](https://www.backblaze.com/blog/hard-drive-cost-per-gigabyte/)

[4. Data Storage Timeline](https://www.frontierinternet.com/gateway/data-storage-timeline/)