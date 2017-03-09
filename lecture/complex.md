---
layout: page
title: "Complex Variable"
image:
  feature: table.jpg
  teaser: table-teaser.jpg
  credit:
  creditlink:
---

Konten:


Pengenalan Bilangan Kompleks 
=================

Rangkuman
---------

Bilangan kompleks $z$ bisa dituliskan dalam bentuk $(x,y)$ dengan $x$
dan $y$ berturut-turut disebut sebagai bagian real dan bagian imaginer
dari $z$; 

$$\textrm{Re}\left( z \right) = x, 
            \qquad \textrm{Im}\left( z \right) = y.$$ 

Penjumlahan dan
perkalian dua bilangan kompleks $z_1 = (x_1,y_1)$ dan $z_2 = (x_2,y_2)$
didefinisikan sebagai berikut: 

$$
\begin{aligned}
     (x_1,y_1) + (x_2, y_2 ) &= (x_1 + x_2, y_1 + y_2) \\
     (x_1,y_1)(x_2,y_2) &= (x_1x_2 - y_1y_2, x_1y_2 + x_2y_1) 
\end{aligned}
$$ 

Modulus dari bilangan kompleks $z=(x,y)$ yang
dinotasikan dengan $|z|$ didefinisikan sebagai bilangan real tak negatif
$|z| = \sqrt{x^2 + y^2}$.

Latihan
-------

1.  Verifikasi perhitungan berikut

    1.  $\left( \sqrt{2}-i\right) -i\left( 1-\sqrt{2}i\right) =  -2i$

    2.  $\left( 2,-3\right) \left( -2,1\right) =\left( -1,8\right) $

    3.  $\left( 3,1\right) \left( 3,-1\right) \left( \frac{1}{5},\frac{1}{10}%
                        \right) =\left( 2,1\right) $

    4.  $\left( \frac{1+\sqrt{5}i}{2}\right) \left( \frac{1-\sqrt{5}i}{2}%
                        \right) =  \frac{3}{2}$

    5.  $\left( 1+i\right) \left( 1+2i\right) \left( 1+4i\right) = 
                        -13-i$

2.  Sederhanakan ekspresi-ekspresi berikut
    $$\frac{1+2i}{3-4i}  + \frac{2-i}{5i}; \qquad 
                    \frac{5i}{(1-i)(2-i)(3-i)}; \qquad 
                    (1-i)^4.$$

3.  Tunjukkan bahwa untuk sebarang bilangan kompleks $z$ berlaku

    1.  $\textrm{Re}\left( iz\right) =-\textrm{Im}\left(z\right)$ dan
        $\textrm{Im}\left( iz\right) =\textrm{Re}\left(z\right)$

    2.  $\left( 1+z\right) ^{2}=  z^{2}+2z+1$

4.  Tunjukkan bahwa

    $
                    (a) \,\, (-1)z=-z \qquad \qquad(b)\,\, \frac{1}{1/z} =z (z\neq 0).
                $

5.  Verifikasi bahwa kedua bilangan $z=1\pm i$ memenuhi persamaan $
            z^{2}-2z+2=0$.

6.  Buktikan bahwa untuk sebarang tiga bilangan kompleks $z_{1}$ dan
    $z_{2}$ berlaku:

    1.  sifat komutatif $$z_{1}z_{2}=z_{2}z_{1}$$

    2.  asosiatif $$(z_1 +z_2) + z_3 = z_1 + (z_2 + z_3) \qquad dan 
                                \qquad (z_1z_2)z_3 = z_1 (z_2z_3)$$

    3.  distributif $$z_1(z_2 + z_3) = z_1z_2 + z_1z_3.$$

7.  Gunakan sifat asosiatif untuk penjumlahan dan sifat distributif
    untuk menunjukkan bahwa $$z(z_1 + z_2 + z_3) = zz_1 + zz_2 + zz_3.$$

8.  Dengan sifat asosiatif dan sifat komutatif perkalian, tunjukkan
    bahwa $$(z_1z_2)(z_3z_4) = (z_1z_3)(z_2z_4)$$

9.  Buktikan bahwa jika $z_1z_2z_3 =0$, maka salah satu faktor adalah
    $0$.

10. Dengan menuliskan $i=(0,1)$ dan $x=(x,0)$, perlihatkan bahwa
    $-(iy)=(-i)y=i(-y)$.

11. Cari solusi dari persamaan $z^2 +z+1=0$ untuk $z=(x,y)$ dengan cara
    menuliskan persamaan tersebut dalam bentuk
    $$(x,y)(x,y)+(x,y)+(1,0)=(0,0)$$ kemudian menyelesaikan sistem
    persamaan dalam $x$ dan $y$ tersebut.

12. Tentukan lokasi bilangan $z_1+z_2$ dan $z_1 -z_2$ dengan vektor jika
    diketahui

    1.  $z_1 = 2i, \quad z_2 = \frac 23 - i$

    2.  $z_1 = (-\sqrt3,1), \quad z_2=(\sqrt 3,0)$

    3.  $z_1 = (-3,1), \quad z_2 = (1,4)$

    4.  $z_1 = x_1 + iy_1, \qquad z_2 = x_1 - iy_1$

13. Buktikan bahwa
    $\sqrt 2\vert z\vert \geq \vert \textrm{Re} \left( z\right) \vert + \vert \textrm{Im}\left(z\right) \vert$.

    Hint : Reduksi persamaan menjadi $ (|x|-|y|)^2\geq 0 $.

14. Pada masing-masing kasus, sketsalah himpunan titik-titik yang
    merupakan tempat kedudukan yang memenuhi kondisi yang diberikan:

    a. $|z-1+i| =1$

    b. $|z+i| \leq 3 

    c. $|z-4i| \geq 4.$

15. Dengan menggunakan bahwa $|z_1 - z_2| $ adalah jarak diantara dua
    titik $z_1$ dan $z_2$, berikan argumen geometris bahwa
    $$|z-1| = |z+i|$$ merepresentasikan garis yang melewati titik asal
    dengan gradien $-1$.


Konjugat Kompleks
=================

Rangkuman
---------

Konjugat kompleks dari bilangan $z=x+iy$ dilambangkan dengan $\bar{z}$,
didefinisikan sebagai $\bar{z}=x-iy$.

### Sifat-sifat

1.  $\overline{\bar{z}}=z$ dan $|\bar{z}|=|z|$.

2.  $\overline{z_1 + z_2} = \overline{z_1} + \overline{z_2}$ dan
    $\overline{z_1 - z_2} = \overline{z_1} - \overline{z_2}$.

3.  $\overline{z_1 z_2} = \overline{z_1} \overline{z_2}$.

4.  $\overline{\left( \frac{z_1}{z_2}\right)} = \frac{\overline{z_1}} { \overline{z_2}}$
    $\qquad$ $\left( z_2 \neq 0\right)$.

5.  $\textrm{Re } z = \frac{z+\bar z}2$ dan
    $\textrm{Im } z = - \frac{z-\bar z }2$.

6.  $z \bar z = | z|^2$ sehingga $\frac 1z = \frac{\bar z }{|z|^2}$ jika
    $z \neq 0$.

7.  $|z_1 z_2 | = |z_1|\ |z_2|$ dan
    $\left \vert \frac{z_1}{z_2} \right \vert = \frac{z_1}{z_2}$

Misalkan koordinat polar $(r,\theta)$ berkorespondensi dengan bilangan
kompleks tak nol $z=x+iy$. Karena $x=r \cos \theta$ dan
$y=r \sin \theta$ maka $z$ bisa dituliskan dalam bentuk
$$z = r(\cos \theta + i \sin \theta).$$ Bilangan real $r$ menyatakan
panjang vektor $z$ sedangkan bilangan real $\theta$ menyatakan sudut
(yang dibentuk dengan sumbu real positif), atau disebut juga ,
dinotasikan dengan . Karena $\sin$ dan $\cos$ adalah fungsi periodik,
maka banyak $\theta$ yang nilai fungsinya sama. Nilai $\theta$, sehingga
$-\pi < \theta \leq \pi $ disebut argumen prinsipal, dan dinotasikan
dengan . Berlaku pula kesamaan

$$\arg z = \text{Arg }z + 2n \pi \qquad (n=0, \pm 1, \pm2, \dots).$$

**Formula Euler**. Simbol $e^{i\theta}$ atau $\exp(i\theta)$ (atau
kadang disebut juga cis $\theta$) didefinisikan sebagai

$$e^{i\theta} = cos \theta + i \sin \theta$$

Perkalian dua bilangan kompleks $z_1 = e^{i\theta_1}$
$ z_2 = e^{i\theta_2}$ menghasilkan

$$z_1 z_2 = e^{i\theta_1} e^{i\theta_2} = e^{i(\theta_1 + \theta_2)}$$

**Formula De Moivre** Untuk bilangan real $\theta$ dan bilangan bulat
$n$ berlaku 

$$\left(e^{i \theta}\right)^n = e^{in\theta}$$ 

atau bisa
ditulis dalam bentuk

$$
	(\cos \theta + i \sin \theta)^n = \cos n \theta + i \sin n\theta.
$$

Latihan
-------

1.  Gunakan sifat-sifat moduli untuk membuktikan bahwa

    1.  $\overline{\bar z + 3i} = z -3i$

    2.  $\overline{iz}=-i\bar z$

    3.  $\overline{(2+i)^2}=3-4i$

    4.  $|(2\bar z + 5)(\sqrt 2 - i)| = \sqrt 3 \ |2z+5|$

2.  Sketsalah masing-masing himpunan titik yang ditentukan dengan
    kondisi berikut


    1.  $\textrm{Re }(\bar z -i)=2$

    2.  $|2z - i| = 4$

3.  Buktikan bahwa
    $\overline{z_1 z_2 z_3} = \overline{z_1}\overline{z_2}\overline{z_3}$
    dan $\overline{z^4} = \overline{z}^4$

4.  Buktikan bahwa jika $z_2$ dan $z_3$ tak kosong, berlaku :


    1.  $\overline{\left( \dfrac {z_1}{z_2 z_3 } \right)} = \dfrac{\overline{z_1}}{\overline{z_2} \ \overline {z_3}}$

    2.  $\left \vert \dfrac{z_1}{z_2 z_3} \right \vert = \dfrac{\vert z_1 \vert}{|z_2| \ |z_3|}$

5.  Untuk setiap bilangan kompleks $z_1,z_2,z_3,z_4$, jika
    $|z_3| \neq |z_4|$,
    $$\left\vert \dfrac{z_1 + z_2}{z_3 + z_4} \right\vert \leq \dfrac{|z_1| + |z_2|}{\left\vert |z_3| - |z_4| \right\vert}.$$

6.  Tunjukkan bahwa
    $| \textrm{Re}(2+\bar z + z^3)| \leq 4 \qquad \textrm{saat } |z| \leq 1 $

7.  Buktikan bahwa jika $|z|=2$ maka berlaku
    $$\left\vert \frac{1}{z^4 - 4z^2 +3} \right\vert \leq \frac 13$$

8.  Tunjukkan bahwa $|z_1 + z_2| \leq (|z_1| + |z_2|)$ dengan
    menguadratkan kedua luas terlebih dahulu dan menunjukkan bahwa
    $z_1\overline{z_2} + \overline{z_1\overline{z_2}} = 2 \textrm{ Re }z_1\overline{z_2} \leq 2 |z_1||z_2|$.

9.  Tentukan argumen prinsipal $z$ jika diketahui:

      

    1.  $z = \dfrac i{-2-2i}$

    2.  $z= (\sqrt3 -i )^6$

10. Tunjukkan bahwa $e^{i\theta}$ = 1. Tunjukkan pula bahwa
    $\overline{e^{i\theta}} = e^{-i\theta} $

11. Dengan menggunakan formula De Moivre, turunkan kesamaan trigonometri
    berikut:

      

    1.  $\cos 3\theta = \cos ^3 \theta - 3 \cos \theta \sin^2\theta$

    2.  $\sin 3 \theta = \cos^2 \theta\sin \theta - \sin^3 \theta$.

12. Jika Re $z_1 >0$ dan Re $z_2$ &gt;0 buktikan bahwa
    $$\textrm{Arg }z_1z_2 = \textrm{Arg }z_1 + \textrm{Arg } z_2.$$

13. Buktikan bahwa dua bilangan kompleks $z_1$ dan $z_2$ mempunyai
    modulus yang sama jika dan hanya jika terdapat bilangan kompleks
    $c_1$ dan $c_2$ sehingga $z_1 = c_1c_2$ dan
    $z_2 = c_1 \overline{c_2}$.

    *Hint:* Tinjau bahwa

    $$\exp(i(\theta_1 + \theta_2)/2) \exp(i(\theta_1 - \theta_2)/2) = \exp(i\theta_1)$$

	dan

    $$\exp(i(\theta_1 + \theta_2)/2) \overline{\exp(i(\theta_1 - \theta_2)/2)} = \exp(i\theta_2)$$.

14. Buktikan identitas berikut untuk $z\neq1$,
    $$1+z+z^2 + \cdots + z^n = \frac{1-z^{n+1}}{1-z}.$$ Buktikan pula
    identitas berikut untuk $0<\theta < 2\pi$,

    $$
	1+ \cos\theta + \cos 2\theta + \cdots + \cos n \theta = \frac 12 + \frac{\sin[(2n+1)\theta /2]}{2\sin (\theta /2)}.
    $$

Akar dari bilangan kompleks
===========================

Rangkuman
---------

Dua bilangan kompleks tak nol $z_1 = r_1 e^{i\theta _1}$ dan
$z_2 = r_2 e^{i\theta _2}$ sama jika dan hanya jika untuk suatu bilangan
bulat $k$.

Jika $z^n = z$ maka
$$z = \sqrt[n]{r_0} \exp \left[ i\left( \frac{\theta _0 }n + \frac{2k \pi}{n}\right) \right] \qquad (k=0,\pm 1, \pm 2,\dots)$$
Semua akar berbeda persamaan tersebut didapat saat $k=0,1,2,\dots, n-1$.
Akar yang memiliki argumen prinsipal disebut .

**Root of Unity** Akar-akar berbeda dari persamaan $z^n = 1$ yaitu
$\exp(i(2k\pi)/n)$ untuk $k=1,2,...,n-1$, disebut *root of unity* dan
dilambangkan dengan 

$$
	1,\omega_n, \omega_n^2,...,\omega_n^{n-1}.
$$ 

Salah
satu sifat yang menarik adalah, jika $c$ adalah salah satu dari *root of
unity*, maka 

$$
	c,c\omega_n, c\omega_n^2,...,c\omega_n^{n-1}.
$$ 

juga
merupakan akar-akar berbeda pada root of unity.


Latihan
-------

1.  Tentukan akar kuadrat dari $2i$ dan $1-\sqrt3 i$ dan nyatakan dalam
    bentuk $a+bi$.

2.  Tentukan masing-masing akar yang diminta pada ekspresi, kemudian
    nyatakan dalam $a+bi$, kemudian tentukan akar prinsipalnya.

    1.  $(-16)^{1/4}$

    2.  $(-8-8\sqrt3 i )^{1/4}$

3.  Pada tiap kasus, tentukan akar yang diminta, nyatakan dalam $a+bi$,
    nyatakan dalam gambar sebagai titik-titik sudut suatu poligon,
    kemudian identifikasi akar prinsipalnya.

    1.  $(-1)^{1/3}$

    2.  $8^{1/6}$

4.  Misalkan pada persamaan $z^n = z_0$, dengan
    $z_0 = -4\sqrt 2 + 4 \sqrt 2 i $. Tentukan ketiga akar prinsipal
    dari persamaan tersebut.

    *Hint :* tiga akar persamaan kubik dapat ditulis sebagai
    $c_0,c_0\omega_3,c_0\omega_3^2$ untuk sebarang akar prinsipal $c_0$.

5.  Buktikan bahwa akar kuadrat dari $a+i$ adalah
    $$\pm \frac 1{\sqrt2} \left( \sqrt{A+a} + i \sqrt{A-a}\right).$$

6.  Tentukan akar pangkat 4 dari $z^4 +4 $ lalu gunakan hasil tersebut
    untuk memfaktorkan $z^4 +4$ menjadi dua faktor dengan
    koefisien real.

7.  Misalkan $c$ adalah root of unity ke-$n$ dengan $c\neq1$, buktikan
    bahwa $$1+ c + c^2 + \cdots + c^{n-1} = 0.$$
