---
layout: post
title: "5 Software yang harus diinstall di Ubuntu"
location: "mesin pc/laptop lokal"
date: 2020-12-10
tags:
 - ubuntu
 - ubuntu LTS
 - ubuntu 20.04
 - software
 - linux
 - firefox
 - chromium
 - google docs
 - sublime text
 - vs code
 - python
 - python3
 - pip
 - install pip
 - virtual environment
 - venv
 - apt-get
 - apt
 - aptitude
 - numpy
 - scipy
 - matplotlib
 - git
 - setting git global
 - vlc
 - rhythmbox
---


# Ubuntu 20.04

Mengunduh Ubuntu 20.04.01 dengan cukup susah payah karena koneksi Indihome yang medioker hanya untuk menemukan bahwa ternyata sudah punya 20.04 LTS di hard drive. Sudah nginstall uTorrent padahal. Tau gitu kan... 

Menginstall Ubuntu tidak sesusah menginstall linux jaman dulu. Sudah cukup mudah, semudah menginstall Windows. Kecuali jika Anda ingin custom. Itu beda cerita. 


Pertama yang dilakukan setelah menginstall Ubuntu adalah menginstall beberapa software utama

## Chromium aka Chrome untuk Linux. 

   Browser utama tetap Firefox. Namun, Firefox adalah browser utama Ubuntu, jadi tidak perlu download lagi. Saya mendownload Chromium sebab perlu menggunakan Google Drive dan Google Docs (offline) untuk pengganti Microsoft Office, salah satu dari 5 software yang saya belum menemukan gantinya di Linux yang cukup nyaman digunakan. Dalam hal ini, Google Docs dan teman-temannya merupakan alternatif yang paling oke diantara yang lainnya. So, disinilah akhirnya mengapa mau mendownload chromium: demi google docs offline. Udah itu aja. 
   
   Ternyata di Chrome nggak punya tab container seperti di Nightly build-nya firefox. :relieved:

## Menginstall text editor. 

![Editor](https://imgs.xkcd.com/comics/real_programmers.png)

   Selain menginstall Sublime-text, saya juga menginstall VS Code. Pengen nyobain aja, katanya orang-orang cukup enak. Liat ntar deh. Eh, tapi ternyata saya ngetik ini via gedit. Lebih clean tampilannya. Cukup lah buat ngetik yang ringan-ringan. 
   
## Menginstall Python dan teman-temannya. 

![Python Environment](https://imgs.xkcd.com/comics/python_environment.png)
	
   Karena ngisntall Ubuntu ini demi simulasi yang jalan di linux dengan Python, jadi memang nginstall Python karena kebutuhan. Guess what, as expected the Python has been installed under the name python3. Unfortunately, it have no pip installed, meanwhile, I need pip to seamlessly install package on python. Then, using comman ```python --version```, I got the version 3.8.2. But, I don't think that this is the last version. But, nevermind, I will install pip anyway. 
   
   Setelah mencari tahu di official page nya pip [https://pip.pypa.io/en/stable/installing/](https://pip.pypa.io/en/stable/installing/), dibilang kalau harusnya sudah ada pip-nya.
   
>  pip is already installed if you are using Python 2 >=2.7.9 or Python 3 >=3.4 downloaded from python.org or if you are working in a Virtual Environment created by virtualenv or venv. Just make sure to upgrade pip.

Namun, sayang sekali ternyata setelah ngecek 

```
~$python3 -m pip --version
/usr/bin/python3: No module named pip
```

tidak ketemu. 

Damn. 


Membaca dokumen official tadi, lalu ada kotak kuning warning besar: 

> Be cautious if you are using a Python install that is managed by your operating system or another package manager. get-pip.py does not coordinate with those tools, and may leave your system in an inconsistent state.

oke. Kita ikutin aja. 

> See the Using Linux Package Managers section if your Python reports No module named ensurepip on Debian and derived systems (e.g. Ubuntu).

Lalu diarahkan ke tempatnya python. [https://packaging.python.org/guides/installing-using-linux-tools/](https://packaging.python.org/guides/installing-using-linux-tools/). Scroll ke bawah, ada section untuk Debian dan Ubuntu. Katanya suruh nginstall dengan 

```
sudo apt install python3-venv python3-pip
```

untuk python3. Got error message. A long one. Disuru masukin media di /cdrom/. Kan bingung ya, orang ini juga nginstall pake usb tadi. 

> Get:1 http://id.archive.ubuntu.com/ubuntu focal-updates/main amd64 cpp-9 amd64 9.3.0-17ubuntu1~20.04 [7.494 kB]                        
> Media change: please insert the disc labeled                                                                                           
>  'Ubuntu 20.04.1 LTS _Focal Fossa_ - Release amd64 (20200731)'
> in the drive '/cdrom/' and press [Enter]

Dan sepertinya harus muter pakai cara lain. Ngubek-ubek dokumentasi bagaimana menginstall pip di debian. Semuanya mengarah ke package manager. Ngga boleh install sendiri. Dan ini artinya harus pake aptitude (apt, apt-get). Sebenarnya, ada opsi untuk manage version via virtual environtment --- venv (Python 3.3+), virtualenv (Python 2), pyvenv (Python < 3.6), --- namun sayangnya semua opsi untuk virtual environment perlu menginstall package sendiri. Dan ini artinya saya harus menginstall package manager. Namun nginstall sendiri, tidak disarankan karena saya nggak mau ribet ngurusin packagae satu-satu nantinya. Mungkin sebenarnya menginstall satu library sendiri tidak masalah apabila nanti sudah menginstall package manager. Tapi sayangnya, saya belum pernah melakukannya. Nggak lucu kan kalau nanti ternyata package manager nggak mau recognize library yang saya install sendiri. 

Kembali ke topik, akhirnya saya melakukan tweak di repository. Yang tadinya selalu minta ```/cdrom/``` saya coba buang. Kabar baiknya adalah, sekarang tampilan ngurusin repository nggak seprimitif dulu. Sudah ada UI nya. :yeay: 

Dan akhirnya bisa menginstall library via pip. 

```
pip3 install numpy scipy matplotlib
```

Selesai? Ternyata tidak :crying: Di suatu bagian tadi saya sepertinya mengeset sesuatu yang saya tidak sadar. 

![gambar]()

Saya coba ngeset PYTHONUSERBASE di ```~/.local/``` lalu nginstall numpy scipy dan matplotlib. DAN keluar warning lagi. Damn. 

![gambar]()

Ya sudah, uninstall lagi deh. Mari kita instal venv karena sudah punya pip3, yang ternyata nggak berhasil juga. Menginstall venv via aptitude (apt, apt-get) masih terasa sangat janggal. :sigh: tapi ya sudahlah, mau bagaimana lagi. 

```
sudo apt install python3-venv
```

dan akhirnya berhasil menggunakan pip. 

Finally. 

## Menginstall git

Menginstall git adalah salah satu yang wajib dilakukan untuk memulai koding dan versioning. Meski saya sendiri belum pernah beneran pake. Tapi (katanya) ini penting. jadi ya saya install aja. Kalau nanti ada masalah waktu memakai git, ya liat nanti. Masih ada stackoverflow, aman lah ya. 

setelah ```git config --global user.email "rud72k@gmail.com"``` dan semuanya selesai.

## Menginstal VLC

Nambah satu software untuk multimedia biar bisa nyetel video. Untuk musik, bawaannya Ubuntu, si Rythmbox, udah cakep, jadi nggak akan diganti-ganti. Untuk video, memilih VLC karena ini paling terkenal (kayaknya). Install via Ubuntu Software juga beres.  :smile:


## Kesimpulan

Di titik ini, yang sudah diinstall adalah:

1. Browser
	- Firefox (default)
		+ Tab container addson
		+ Youtube downloader addson
	- Chromium
		+ Google Drive Offline
		+ Youtube Analytics
		+ Youtube donwloader plugins
2. Teks Editor
	- GEdit (default)
	- Sublime Text 3
	- VS Code
3. Python
	- Python3 (default)
	- pip3 via aptitude (apt install python3-pip)
	- venv via aptitude (apt install python3-venv)
	- numpy, scipy, matplotlib via pip (di dalam venv)
4. git
	- ngeset global variabel:
		- ```git config --global user.email "emailsaya@manapun.com"``` 
		- ```git config --global user.name "Rudi Prihandoko"
5. Multimedia
	- Rhythmbox
	- VLC
	
Yang akan diinstall tapi belum:
1. Texlive (latex engine)
2. ANUGA via github demi kepentingan umat
3. Darkroom (semacam lightroom-nya adobe)
4. Autodesk Sketchup untuk menggambar

Terakhir, sebelum tulisan ini ditutup, saya ngeclone repo github untuk mengupdate tulisan ini.
