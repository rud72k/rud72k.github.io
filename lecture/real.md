---
layout: page
title: "Introduction to Real Analysis"
image:
  feature: room.jpg
  teaser: room-teaser.jpg
  credit:
  creditlink:
---

## [Daftar Isi](/)

- [Pointwise and Uniformly Convergent](#pointwise-and-uniformly-convergen)
    - [Rangkuman](#rangkuman)
    - [Latihan](#latihan)
- [Interchange of Limit](#interchange-of-limit)
    - [Rangkuman](#rangkuman-2)
    - [Latihan](#latihan-2)
- [Metrik](#metrik)
    - [Rangkuman](#rangkuman-3)
    - [Latihan](#latihan-3)


Pointwise and Uniformly Convergen
=====================

Rangkuman
---------

**Definisi** Misalkan $(f_n)$ adalah barisan fungsi yang terdefinisi di
$A\subseteq \mathbb{R}$ dan $A_0 \subseteq A$. Misalkan pula
$f:A \rightarrow \mathbb{R}$. Barisan $(f_n)$ dikatakan konvergen di
$A_0$ ke $f$ jika untuk setiap $x\in A_0$, barisan $(f_n(x))$ konvergen
ke $f(x)$ di $\mathbb{R}$. Pada kasus ini $f$ disebut sebagai limit dari
barisan $(f_n)$ di $A_0$. Jika fungsi $f$ yang demikian ada, maka
$(f_n)$ dikatakan konvergen di $A_0$ atau $(f_n)$ konvergen
titik-demi-titik di $A_0$.

**Teorema** Suatu barisan fungsi $(f_n)$di $A\subseteq \mathbb{R}$ konvergen ke
fungsi $f:A_0 \rightarrow \mathbb{R}$ jika dan hanya jika untuk setiap
$\epsilon >0$ dan untuk setiap $x\in A_0$ terdapat bilangan asli
$K(\epsilon,x)$ sedemikian hingga jika $n\geq K(\epsilon,x)$ maka
berlaku 

$$
    \vert f_n(x)-f(x)\vert < \epsilon.
$$

**Definisi** Suatu barisan fungsi $(f_n)$ pada $A\subseteq \mathbb{R}$ konvergen
seragam pada $A_0 \subseteq A$ ke fungsi $f:A\rightarrow \mathbb{R}$
jika untuk setiap $\epsilon >0$ terdapat bilangan asli $K(\epsilon)$
(bergantung hanya pada $\epsilon$, tidak pada $x$)sedemikian hingga
untuk setiap $n\ge K(\epsilon)$ berlaku

$$\vert f_n(x)  - f(x) \vert < \epsilon \qquad \forall x\in A_0.$$ 

Pada
kasus demikian kita katakan $(f_n)$ konvergen seragam ke $A_0$.

**Teorema** Suatu barisan fungsi $(f_n)$ di $A\subseteq \mathbb R$ tidak konvergen
seragam di $A_0 \subseteq A$ ke fungsi $f:A\rightarrow \mathbb R$ jika
dan hanya jika untuk suatu $\epsilon_0 >0$ terdapat subbarisan
$(f_{n_k})$ dari $(f_n)$ dan suatu barisan $(x_k)$ di $A_0$ sehingga

$$\vert f_{n_k} (x_k) - f(x_k) \vert \geq \epsilon_0 \qquad \forall k\in \mathbb{N}$$

**Definisi** Misalkan $A\subseteq \mathbb R$ dan $\varphi:A \rightarrow \mathbb R$
adalah suatu fungsi. Fungsi $\varphi$ dikatakan terbatas di $A$ jika
himpunan $\varphi(A)$ adalah subset terbatas di $\mathbb R$. Jika
$\varphi$ terbatas, didefinisikan norma seragam pada $\varepsilon$ di
$A$ dengan

$$\Vert \varphi \Vert_A := \sup \{ \vert \varphi (x)\vert : x\in A\}.$$

**Teorema** Suatu barisan terbatas $(f_n)$ di $A\subseteq \mathbb R$ kovergen
seragam di $A$ ke $f$ jika dan hanya jika
$\Vert f_n -f \Vert_A \rightarrow 0$.

**(Kriteria Cauchy untuk kekonvergenan seragam)** Misalkan $(f_n)$
adalah barisan fungsi terbatas di $A\subseteq \mathbb R$. Maka barisan
ini konvergen seragam ke suatu fungsi terbatas $f$ jika dan hanya jika
untuk setiap $\epsilon >0$ terdapat bilangan $H(\epsilon)$ di
$\mathbb N$ sehingga untuk setiap $m,n \geq H(\epsilon)$, berlaku
$\Vert f_m - f_n \Vert_A \leq \epsilon$.

Latihan
-------

1.  Tunjukan bahwa $\lim(x/(x+n))=0$ untuk setiap $x\in \mathbb R, x\geq 0$. 

2.  Tunjukan bahwa $\lim(nx/(1+n^2x^2))=0$ untuk setiap $x\in \mathbb R$. 

3.  Tentukan $\lim(nx/(1+nx))$ untuk setiap $x\in \mathbb R, x\geq 0$.

4.  Tentukan $\lim(x^n/(1+x^n))$ untuk setiap $x\in \mathbb R, x\geq 0$.

5.  Tentukan $\lim((\sin nx)/(1+nx))$ untuk setiap $x\in \mathbb R, x\geq 0$. 

6.  Tunjukan bahwa $\lim(\arctan nx) = (\pi/2) \cdot \sgn(x)$. 

7.  Evaluasi nilai $\lim (e^{-nx})$ untuk suatu $x\in \mathbb{R}$, $x\ge 0$. 

8.  Tunjukkan bahwa $\lim(xe^{-nx})=0$ untuk $x\in \mathbb R$, $x\ge 0$.

9.  Tunjukkan bahwa $\lim(x^2e^{-nx})=0$ dan $\lim(n^2x^2e^{-nx})=0$ untuk $x\in \mathbb R,x\ge 0$. 

10. Tunjukkan bahwa $\lim\left((\cos \pi x)^{2n} \right)$ ada untuk
    setiap $x \in \mathbb R$. Tentukan nilai limit tersebut. 

11. Tunjukkan bahwa jika $a>0$ maka konvergensi pada (1) adalah
    konvergen seragam pada interval $[0,a]$, tapi tidak konvergen
    seragam pada interval $[0,\infty)$.

12. Tunjukkan bahwa jika $a>0$ maka konvergensi pada (2) adalah
    konvergen seragam pada interval $[a,\infty)$, tapi tidak konvergen
    seragam pada interval $[0,\infty]$.

13. Tunjukkan bahwa jika $a>0$ maka konvergensi pada (3) adalah
    konvergen seragam pada interval $[a,\infty)$, tapi tidak konvergen
    seragam pada interval $[0,\infty]$.

14. Tunjukkan bahwa jika $0 < b < 1 $,maka konvergensi pada (4)
    konvergen pada interval $[0,b]$ tapi tidak konvergen pada interval
    $[0,1]$.

15. Tunjukkan bahwa jika $ a >0$ maka konvergensi pada (5) adalah
    konvergen seragam pada interval $[a,\infty)$, tapi tidak konvergen
    seragam pada interval $[0,\infty]$.

16. Tunjukkan bahwa jika $a>0$ maka konvergensi pada (6) adalah
    konvergen seragam pada interval $[a,\infty)$, tapi tidak konvergen
    seragam pada interval $(0,\infty]$.

17. Tunjukkan bahwa jika $a>0$ maka konvergensi pada (7) adalah
    konvergen seragam pada interval $[a,\infty)$, tapi tidak konvergen
    seragam pada interval $[0,\infty]$.

18. Tunjukkan bahwa konvergensi pada (8) adalah konvergen seragam
    pada $[0,\infty)$.

19. Tunjukkan bahwa barisan $(x^2 e^{-nx})$ konvergen seragam pada
    $[0,\infty)$.

20. Tunjukkan bahwa jika $a>0$, maka barisan $(n^2 x^2 e^{-nx})$
    konvergen seragam pada interval $[a,\infty)$ tapi tidak konvergen
    seragam pada inverval $[0,\infty)$

21. Tunjukkan bahwa jika $f(x)=x+1/n$ dan $f(x)=x$ untuk setiap
    $x\in \mathbb R$ maka $(f_n)$ konvergen seragam di $\mathbb R$ ke
    $f$, tapi $(f_n^2)$ tidak konvergen seragam di $\mathbb R$.

22. \[jumlahseragam\] Tunjukkan bahwa jika $(f_n)$ dan $(g_n )$
    konvergen seragam pada himpunan $A$, berturut-turut ke fungsi $f$
    dan $g$, maka barisan $(f_n + g_n)$ konvergen seragam pada himpunan
    $A$ ke fungsi $f+g$.

23. \[kaliseragam\] Tunjukkan bahwa jika $(f_n)$ dan $(g_n )$ barisan
    fungsi terbatas yang konvergen seragam pada himpunan $A$,
    berturut-turut ke fungsi $f$ dan $g$, maka barisan $(f_ng_n)$
    konvergen seragam pada himpunan $A$ ke fungsi $fg$.

24. Misalkan $(f_n)$ adlaah fungsi yang konvergen seragam ke $f$ di $A$
    dan memenuhi $\vert f_n (x) \vert \le M$ untuk setiap
    $n\in \mathbb N $ dan setiap $x \in A$. Jika $g$ kontinu pada
    interval $[-M,M]$, tunjukkan bahwa barisan $(g\circ f_n)$ konvergen
    seragam ke $g \circ f$ pada $A$.


Interchange of Limit
====================

Rangkuman
---------

**Teorema** Misalkan $(f_n)$ adalah barisan fungsi kontinu pada himpunan
$A \subseteq \mathbb R$ dan misalkan pula $(f_n)$ konvergen seragam ke
suatu fungsi $f:A \to \mathbb R$. Maka $f$ kontinu di $A$.

**Teorema** Misalkan $J \subseteq \mathbb R$ adalah interval terbatas dan $(f_n)$
adalah barisan fungsi pada $J$ ke $R$. Misalkan terdapat $x_0 \in J$
sehingga $(f_n (x_0))$ konvergen, dan barisan turunan fungsi
$(f_n^{\prime})$ ada di $J$ dan konvergen seragam di $J$ ke suatu fungsi
$g$. Akibatnya, barisan fungsi $(f_n)$ konvergen seragam di $J$ ke suatu
fungsi $f$ yang punya turunan di setiap titik di $J$ dan $f^{\prime}=g$.

**Teorema** Misalkan $(f_n)$ adalah barisan fungsi di $R[a,b]$ dan misalkan
pula $(f_n)$ konvergen seragam pada $[a,b]$ ke suatu fungsi $f$.
Akibatnya $f\in R[a,b]$ dan berlaku

$$\int_a^b f = \lim_{n \to \infty} \int_a^b f_n.$$

**(Teorema Konvergen Terbatas)** Misalkan $(f_n)$ adalah barisan fungsi
di ${R}[a,b]$ yang konvergen pada \[a,b\] ke suatu fungsi
$f\in [a,b]$. Misalkan pula terdapat $B>0$ sedemikian hingga
$\vert f_n(x)\vert \leq B$ untuk semua $x\in [a,b],n\in \mathbb N$, maka
berlaku 

$$\int_a^b f = \lim_{n \to \infty} \int_a^b f_n.$$

**(Teorema Dini)** Misalkan $(f_n)$ adalah barisan fungsi kontinu yang
monoton pada interval terbatas $I$ yang konvergen di $I$ ke suatu fungsi
$f$. Maka kekonvergenan barisan tersebut adalah konvergen seragam.

Latihan
-------

1.  Tunjukan barisan $(x^n/(1+x^n))$ tidak konvergen seragam di selang
    $[0,2]$ dengan memperlihatkan bahwa limit fungsi tersebut tidak
    kontinu di $[0,2]$.

2.  Buktika bahwa barisan (1) adalah barisan fungsi kontinu tidak
    seragam ke suatu fungsi kontinu.

3.  Konstruksi suatu barisan fungsi di $[0,1]$ yang masing-masing
    diskontinu di setiap titik di $[0,1]$ yang konvergen seragam ke
    suatu fungsi yang kontinu di setiap titik.

4.  Misalkan $(f_n)$ adalah barisan fungsi kontinu di interval $I$ yang
    konvergen seragam di $I$ ke suatu fungsi $f$. Jika $(x_n) \in I$
    konvergen ke $x_0 \in I$, buktikan bahwa $\lim (f_n (x_n))=f(x_0)$.

5.  Misalkan $f : \mathbb R \to \mathbb R$ kontinu seragam di
    $\mathbb R$ dan misalkan $f_n(x)=f(x+1/n)$ untuk $x \in \mathbb R$.
    Tunjukkan bahwa $(f_n)$ konvergen seragam di $\mathbb R$ ke $f$.

(TO BE CONTINUED!)

Metrik
======

Rangkuman
---------

Pada himpunan tak kosong $X$, suatu fungsi
$d : X \times X \to \mathbb R$ disebut metrik jika untuk sebarang $x,y$
dan $z$ di $X$ berlaku:

1.  $d(x,y) \ge 0$

2.  $d(x,y) = 0 \iff x=y$

3.  $d(x,y) = d(y,x)$

4.  $d(x,y) + d(y,z) \geq d(x,z)$.

Suatu himpunan tak kosong yang dilengkapi metrik disebut ruang metrik.

Pada ruang linear $X$, suatu fungsi real $\| \cdot \|$ yang bernilai tak
negatif disebut norma jika untuk setiap $u$ dan $v$ di $X$, dan sebarang
$\alpha$ di lapangan (*(*underlying field)), berlaku:

1.  $\| u \| =0 \iff u=0$

2.  $\| u+v \| \leq \|u \| + \|v \|$

3.  $\|\alpha u \| = |\alpha| \|u \|$

Dari suatu norma pada ruang linear bisa dibuat metrik dari norma
tersebut (kadang disebut metrik terinduksi) dengan mendefinisikan

$$d(x,y) = \| x - y \|$$

Dua metrik $\rho$ dan $\sigma$ pada $X$ dikatakan ekuivalen jika
terdapat $m$ dan $M$ sehingga
$$m \cdot \sigma (x,y) \leq \rho (x,y) \leq M \cdot \sigma(x,y)$$ untuk
sebarang $x$ dan $y$ di $X$.

Suatu pemetaan dari ruang metrik $(X,\rho)$ ke ruang metrik $(Y,\sigma)$
disebut isometri jika memenuhi 

$$\sigma(f(x_1),f(x_2))=\rho(x_1,x_2)$$


Latihan
-------

1.  Buktikan bahwa fungsi-fungsi berikut adalah suatu metrik di
    $\mathbb R$

    1.  $d(x,y) = |x-y|$

    2.  $d(x,y) = \sqrt{|x-y|}$

2.  Buktikan bahwa fungsi-fungsi berikut adalah suatu metrik di
    $\mathbb R^n$.

    $$\rho(x,y) = |x_1 - y_1| + |x_2 - y_2 | + \cdots + |x_n - y_n|;$$

    $$\sigma(x,y) = \max\{ |x_1 - y_1| + |x_2 - y_2 | + \cdots + |x_n - y_n|\}$$

3.  Tunjukkan bahwa dua metrik $\sigma$ dan $\rho$ pada himpunan $X$
    ekuivalen jika dan hanya jika terdapat $c>0$ sehingga untuk setiap
    $u,v \in X$ berlaku
    
    $$\frac 1c \sigma(u,v) \leq \rho (u,v) \leq c   \sigma (u,v)$$

4.  Tunjukkan bahwa untuk sebarang $a,b,c \ge 0$ sehingga $a \le b+c$
    berlaku 

    $$\frac a{1+a} \leq \frac b{1+b} + \frac c{1+c}$$

5.  Jika $(X,d)$ adalah ruang metrik dan $d^\*(x,y) = d(x,y)/(1+d(x,y))$
    perlihatkan bahwa $(X,d^\*)$ juga ruang metrik. Perlihatkan pula
    bahwa untuk $d_{1/2}(x,y) = \sqrt{d(x,y)}$, maka $(X,d_{1/2})$
    merupakan ruang metrik.

6.  Ditinjau koleksi ruang metrik $$\{(X_n,d_n)\}_{k=1}^{N}$$.
    Didefinisikan fungsi $d$ pada produk kartesian $X=\Pi_{k=1}^N X_k$ dengan

    $$d(x,y) = \sum_{k=1}^N \frac 1{2^n} \frac{d(x,y)}{1+d(x,y)}$$

    dengan $x=(x_1,x_2,...,x_n)$ dan $y=(y_1,y_2,...,y_n)$ di $X$.
    Buktikan bahwa $(X,d)$ adalah ruang metrik.

7.  Jika $(X,d)$ adalah suatu ruang metrik, buktikan bahwa $(X,d^\*)$
    dengan 

    $$d^*(x,y) = \min \{ 1, d(x,y)\}$$ 

    juga merupakan
    ruang metrik.

8.  Ditinjau fungsi 

    $$
        d(x,y) =  
            \begin{cases}
                |x_1 - y_1|                     & \textrm{if } x_2 = y_2 \\
                |x_1| + |x_2 - y_2| + |y_1|     & \textrm{if } x_2 \neq y_2
            \end{cases}
    $$ 

    untuk sebarang $(x_1,x_2)$ dan
    $(y_1,y_2)$ di $\mathbb R^2$. Perlihatkan bahwa $(\mathbb R^2,d)$
    adalah ruang metrik.

9.  Misalkan $X$ adalah himpunan semua fungsi kontinu dari $[a,b]$ ke
    $\mathbb R$. Untuk setiap $x,y$ di $X$, didefinisikan

    $$d(x,y) = \max\{ |x(t) - y(t)| : t \in [a,b]\}$$ 

    Buktikan bahwa
    $(X,d)$ adalah ruang metrik.

10. Misalkan $X$ adalah himpunan semua fungsi kontinu dari $[a,b]$ ke
    $\mathbb R$. Untuk setiap $x,y$ di $X$, didefinisikan

    $$d(x,y) = \int_a^b |x(t)-y(t)| \ dt.$$ 

    Buktikan bahwa $(X,d)$
    adalah ruang metrik.

11. Pada interval tutup $[a,b]$ ditinjau himpunan fungsi kontinu
    bernilai real $C[a,b]$. Tunjukkan bahwa metrik yang diinduksi oleh
    norma maksimum dan yang diinduksi oleh $L^1[a,b]$ tidak ekuivalen.

12. Misalkan $X$ adalah himpunan semua fungsi terbatas dari suatu
    himpunan $A$ ke $\mathbb R$. Untuk sebarang $x,y$ di $X$,
    didefinisikan 

    $$d(x,y) = \sup \{ |x(t) - y(t)| : t\in A\}$$ 

    Buktikan
    bahwa $(X,d)$ adalah ruang metrik.

13. Misalkan $(X,d)$ adalah ruang metrik. Misalkan $p$ adalah titik di
    $X$. Metrik $d_p$ pada $X$ didefinisikan dengan 

    $$d_p(x,y)=
                            \begin{cases}
                                0                   & \textrm{if } x=y \\
                                d(x,p) + d(y,p)     & \textrm{if } x \neq y
                            \end{cases}$$ 

    Buktikan bahwa $(X,d_p)$  adalah ruang metrik.

14. Metrik $d$ pada ruang metrik $(X,d)$ disebut *ultrametrik* jika berlaku
    
    $$d(x,y) \le \max\\{d(x,z),d(z,y)\\}$$
    
    untuk sebarang $x,y,z \in X$.

    1.  Tunjukan bahwa metrik Euclid di $\mathbb R^n$, untuk $n \ge 2$
        bukan merupakan ultrametrik.

    2.  Misalkan $p$ adalah sebarang bilangan prima $p \ge 2$. Untuk
        sebarang bilangan tak nol $x\in \mathbb Q$, terdapat bilangan
        bulat $n$ sehingga $$x = p^n \frac u v$$ untuk suatu $u$ dan $v$
        yang tidak habis dibagi $p$. Definisikan $|x|_p = n$. Tunjukkan
        bahwa 

        $$d_p (x,y) = 
                                    \begin{cases}
                                        0                   & \textrm{jika }x=y \\
                                        p^{-|x-y|_p}        & \textrm{jika }x \neq y
                                    \end{cases}$$ 

        adalah suatu
        ultrametrik di $\mathbb Q$.
        Metrik ini disebut juga metrik $p$-adic.

    3.  Jika $(X,d)$ adalah ultrametrik, tunjukan bahwa setiap segitiga
        di $X$ adalah segitiga samakaki. Tunjukkan pula bahwa setiap
        titik pada bola, adalah pusat bola tersebut.