---
layout: post
title: "Instalasi Windows, Browser dan Persaingan"
location: "Windows"
tag:
- Windows
- Firefox
- Chrome
- Edge
- laptop
- Dell
- baru
- Inspiron
- 7460
- i5-7200
- GT 940MX
---

Setelah laptop lama saya pensiun dengan terpaksa, saya akhirnya memutuskan untuk membawa pulang Dell Inspiron 7460 <sup id="f1">[1](#inspiron7460)</sup>. Meski tidak terlalu powerful (karena emang nggak dipake buat yang berat-berat), namun nggak cupu-cupu amat lah. Setelah sok-sokan menghapus partisi windows dan memasang debian jessie, bertemulah dengan masalah bahwa:
leptop ini dual vga pake teknologi optimus yang mana linux belum ada support _resmi_ nya. Maksud saya, bisa sih pakai bumblebee (debian based), cuman yaitu, harus manual satu2 kalau mau menjalankan si nvidia. Di satu sisi bener-bener pengen balik lagi ke linux, di sisi lain `lsusb -l` dan `lspci -l` nya jessie nggak memunculkan kata nvdia sama sekali. Yaudah nyerah deh. 
Eh belum ding, sempat nyobain ubuntu live, dan `lspci -l` nya ubuntu mau mendeteksi si gpu. Tapi apa boleh dikata, nasi sudah menjadi bubur, sekalian aja di kecapi biar nikmat. Akhirnya dengan terpaksa clbk ke windows lagi. 

DAAAAAN..... saya menguras kuota harian donlot dengan mengupdate windows, setelah sebelumnya donlot iso windows di miror kampus. Kampus saya kerjasama dengan Microsoft btw. Beliau memberikan 
kampus kami jendela dengan edisi _home_, _pro_, dan _education_. Bedanya apa? Sok, silakan gugling sendiri. Oh iya, saya akhirnya memakai versi Education (bawaan lepi aslinya hanya yang pro).

Setengah jam pertama instal windows, saya merasa kalau ini windows nggak nyaman banget di mata (setidaknya di leptop FHD ini, di leptop saya yang lama baik-baik saja). Sekalian liat-liat update terbaru ransomware yang lagi ngehits beberapa waktu yang lalu, saya akhirnya memutuskan untuk mengupdate windows ke versi yang paling paling paling baru yaitu versi Mei. Di notifikasinya sih ada yang masih _experimental_ atau entah apa istilahnya kemaren. Dalam hati sih, nggak ngerti, udah next next next aja. Dan tahukah Anda berapa lama saya beres mengunduh (download) dan memasang (install) pembaruan (update) windows terbaru ini? Empat jam saudara-saudara. Empat jam. Satu jam untuk mengunduh di belakang layar atau background (yang mana nggak jadi prioritas), dan tiga jam yang cukup melelahkan melihat si angka persenan instal nggak naek naek. Tiga jam pemasangan daripada idle, saya sekalian mengunduh Microsoft ovis karena kebetulan kami dapat lisensi juga. Jatohnya jadi aseli dong :stuck_out_tongue:. Setelah beres donlot instal donlot instal, saya mulai melihat-lihat fitur windows ini. 

And yes, the updates worth every penny spent. (Yaiyalah, nol rupiah)


Tampilan windows 10 versi terakhir jauh lebih oke dari yang standar. Atau mungkin ini hanya bayangan saya saja. Karena saya lupa nggak skrinsut windows 10 awal, jadi saya nggak memberi perbandingan disini. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/desktop1.png)

Klik tombol start mungkin Anda-anda sudah biasa. Nggak perlu saya skrinsutkan. Tapi klik kanan tombol start memunculkan menu baru yang dulu tidak ada dan kebetulan saya sering memakainya (dulu pas sedang pake windows). Jadi buat saya ini suatu keuntungan. 
Panel kanan pun cukup informatif dibandingkan sebelum update. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/desktop2.png)

(gambar ini diskrinsut belakangan)

Kalau yang pernah menginstal windows sendiri akan sadar bahwa diawal-awal si windows agak menyebalkan dalam mengenalkan software asistennya yang semacam Jarvis-nya Iron Man.
Meski saya non aktifkan, tapi saya penasaran jadi saya coba search dengan memencet tombol windows dan mengetikkan "siri" <sup id="f2">[2](#inspiron7460)</sup>

dan tebaklah apa yang muncul. 

>  Cortana and Search Setting

Kata "siri" dan "cortana" hanya memiliki satu kesamaan huruf, yaitu "r". Itu pun tidak di awal melainkan di tengah. Indikasi persaingan tidak sehat. Hahahaha.. 

Tapi mungkin ini sah-sah saja sih. Toh windows dan cortana di dalamnya merupakan produk Microsoft sedangkan Siri adalah produk Apple, saingan Microsoft. But still it leaves bad aftertaste. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/desktop3.png)

Next. Next.


Hal berikutnya yang saya lakukan adalah mencari berkas instalasi rubah api dan pokeball-like browser. Tentu saja saya ogah memakai IE11. Untungnya di windows 10 ada yang namanya Edge. Yang, sejauh ingatan saya, sangat cepat. Dan baiklah saya mengeklik gambar si Edge. Anda tau apa yang muncul?
Salam selamat datang yang,... Ah, anda bisa lihat sendiri. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/edge1.png)

Another (almost) black campaign. Yasudahlah. 

Lalu saya mengetikkan `firefox download' di kolom alamat. Bagi Anda yang suka berganti-ganti browser pasti paham bahwa fitur pencarian di banyak browser jaman sekarang sudah langsung diimbuhkan ke dalam kolom alamat. Jika itu adalah url atau uri atau ip address, si browser akan langsung menuju halaman tersebut. Jika si browser merasa itu bukanlah salah satu yang dimaksud tadi, maka ia akan melanjutkannya ke mesin pencari. Such a nice feature. Keep a good job, modern browser.

Di masa lalu, pencarian 'bla-bla-bla download' akan mengarah ke halaman resmi yang dilanjutkan dengan salah satu laman download dari halaman resmi. Namun sepertinya hal ini tidak berlaku untuk Bing dan Edge yang kolaborasi dengan windows 10. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/edge2.png)

Such a coward move!

Sembari menginstall firefox, saya mengunduh chrome. Kali ini tidak se-savage firefox. Chrome mungkin tau bahwa dia akan disabotasi oleh musuhnya, jadi ia membeli iklan chrome ke bing, mungkin juga ke google (otomatis lah ini), dan juga ke mesin-mesin pencari lain. Bahkan pencarian via bing (terintegrasi dengan edge by default) menghasilkan satu kolom profile chrome di satu kolom kanan hasil dari pencarian. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/edge3.png)

Sementara langkah yang diambil edge sampai segila itu, ternyata si firefox adem ayem saja. Buktinya ketika pertama kali masuk firefox, ia hanya meminta menjadi default dan tidak ribut ketika saya pilih pilihan not now. Tampilan awal firefox pun cukup adem. Tidak provokatif. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/firefox1.png)

dan saya suka backgroundnya :) 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/firefox2.png)

Kebetulan selama ini saya memang pengguna setia firefox. Seenggaknya sampai tulisan ini dibuat. Langkah penginstallan chrome hanyalah untuk mengetes laman web, apakah konsisten di banyak browser atau tidak. (Sori safari, opera, dlsb, giliran kalian belum ya). Dan dari ketiga browser ini, chrome lah yang pantas menyandang gelar paling savage. Kalau firefox hanya minta default browser, si edge hanya bilang dia lebih unggul, kalau chrome berani nyuruh-nyuruh penggunanya dan mencampakkan musuhnya. 

![desktop]({{ site.url }}{{ base.url }}/images/post/2017/6/chrome1.png)

Ah I'm not gonna using it in the near future anyway.


Thanks for reading, dan silakan berikan opini apa browser kesukaan Anda di kolom komentar. We'll glad to hear your opinion!

<hr>

<b id="inspiron7460">1</b>: Kaby Lake i5-7200 2.50 GHz --- 4GB RAM --- GT 940MX 4GB --- SSD 128 + HDD 500GB --- FHD 13.3" [↩](#f1)

<b id="siri">2</b>: Bagi Anda yang tidak tahu, Siri adalah perangkat lunak buatan Apple yang fungsinya sama dengan Jarvis tadi.  [↩](#f2)

