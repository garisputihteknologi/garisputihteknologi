1. "Rock Bottom" Sistem Telekomunikasi 5G
==========================================
**Garis Putih Teknologi**

*Menghapus Batas Aksesibilitas*

*Tokyo, 3 Juni 2024*

Membaca kalimat sistem telekomunikasi mungkin membuat beberapa GPT-ID cemas dan ketar-ketir duluan. Kalimat yang sangat identik dengan sistem yang rumit dan teknologi yang kompleks ini menjadi momok menakutkan bagi beberapa rekan, bahkan bagi penulis sendiri. Masih teringat jelas ketika penulis menempuh studi sarjana dahulu, mata kuliah Dasar Sistem Telekomunikasi menjadi mata kuliah yang paling banyak "meninggal-kelaskan" mahasiswa dan menjadi salah satu mata kuliah wajib yang -kalau bisa- lulus saja sudah cukup. Penulis juga ingat ketika kami mahasiswa berbondong-bondong untuk mengambil kelas yang dosennya sangat dermawan memberikan nilai, sehingga kelas tersebut ditutup karena *over capacity*. Pada topik pendahuluan ini, penulis ingin memberikan sedikit dan sekilas gambaran bagaimana arsitektur sistem telekomunikasi 5G secara garis besar dan komponen apa saja yang ada didalamnya.

1. 1. Selayang Pandang Sistem 5G
---------------------------------
Pada sistem telekomunikasi 5G, ada tiga komponen pembentuk yang perlu GPT-ID pahami, pertama adalah perangkat pengguna atau yang bisa disebut sebagai *User Equipment* (UE), perangkat radio atau *Radio Access Network* (RAN), dan perangkat manajemen jaringan atau *Core Network* (CN). Ketiga komponen ini memiliki fungsinya masing-masing dan menjadi komponen utama dalam membentuk satu kesatuan arsitektur sistem telekomunikasi 5G. Secara garis besar arsitektur sistem 5G tergambar pada Gambar 1 dibawah ini.

.. image:: gambar/1_Arsitektur_5G.png
  :width: 800
  :alt: Gambar 1. Arsitektur Sistem Telekomunikasi 5G.
  :align: center

.. centered::
  Gambar 1. Arsitektur Sistem Telekomunikasi 5G.
   
**Perangkat Pengguna (UE)**
Perangkat pengguna atau UE adalah perangkat yang terletak di sisi pengguna, baik yang terhubung secara langsung maupun tidak langsung dengan jaringan 5G dan dapat mengakses layanan sesuai dengan paket kebijakan (*policy*) yang telah dilanggan (*subscribe*). Jenis kebijakan yang dilanggan tergantung dengan kualitas layanan (*Quality of Service*) yang telah disetujui bersama antara pengguna dan provider sistem telekomunikasi. Kualitas layanan ini dapat meliputi *bandwidth*, *latency*, *packet loss*, dan lain sebagainya yang akan dibahas pada topik catatan teknis Kualitas Layanan Jaringan (QoS). Selain itu, kualitas layanan ini juga bergantung dengan studi kasus yang akan diimplementasikan seperti Ultra Reliable and Low Latency Communications (URLLC), enhanced Mobile Broadband (eMBB), atau massive-Machine Type Communications (mMTC) (topik ini juga dibahas lebih detail di topik catatan teknis lain). Kompleksitas kebutuhan yang semakin tinggi atas jaringan selular di 5G, membuat definisi "Perangkat Pengguna" meluas, tidak hanya handphone maupun tablet, tapi juga dapat berupa sensor, perangkat dijital, mobil, hingga mesin perkakas.

**Perangkat Radio (RAN)**
Perangkat radio atau Radio Access Network (RAN) adalah perangkat nirkabel yang menghubungkan perangkat pengguna dengan Perangkat Manajemen Jaringan (CN). Pada teknologi 4G, perangkat ini disebut dengan *evolved Node-B* (eNB) dengan "B"-nya mengacu pada Base Station. Dengan berkembangnya teknologi LTE, terminologi ini kemudian berubah pada sistem telekomunikasi 5G menjadi *5G Next Generation Base Station* atau yang biasa disingkat dengan gNB. GPT-ID tidak perlu memusingkan dengan semua terminologi ataupun penyebutan nama yang sulit ini. Keduanya memiliki fungsi yang sama yaitu meneruskan paket data dari pengguna ke internet, maupun sebaliknya. Perangkat radio ini secara garis besar terbagi menjadi tiga sub bagian, *Antenna*, *Radio Unit* (RU), dan *Baseband Unit* (BBU). Kita akan bahas lebih detail terkait topik ini di di topik catatan teknis Perangkat Radio.

**Perangkat Manajemen Jaringan (CN)**
Perangkat Manajemen Jaringan atau Core Network (CN) adalah komponen arsitektur 5G yang memiliki fungsi untuk mengelola akses bagi perangkat pengguna dan juga radio. Perangkat ini terdiri dari banyak submodul yang terpasang didalamnya seperti AMF, SMF, NSSF, UDM, UPF, dan lain-lain. Masing-masing submodul memiliki fungsinya sendiri-sendiri dan saling berkaitan satu sama lain, baik ketika UE memulai interkoneksi, otorisasi layanan, berselancar di internet, hingga koneksi UE terputus.