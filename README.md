# transceiver-SSB-hf
Ayo belajar merakit transceiver SSB HF



Skip to navigation
Skip to main content
Skip to primary sidebar
Skip to secondary sidebar
Skip to footer
J.A.G.A.W.A.N.AMendalami Homebrew Radio Amatir !
HOME
ABOUT
Facebook
Blog Archives
VFO NE602
NOV 6

Posted by YD1HXJ - jagawana
Iklan

Rasa penasaran ingin membuat VFO yang stabil membawa saya kepada pencarian rangkaian VFO menggunakan IC. Saya sudah mencoba menggunakan TA7358 tetapi hasilnya kurang memuaskan dimana frekuensi VFO meloncat-loncat tidak teratur sehingga tidak saya lanjutkan. Kebetulan saya mendapat hibah IC NE602 / SA602 dari pak Indra S. Ekoputro yang merupakan IC multiguna untuk RF, yang katanya menurut literatur bisa juga dirangkai menjadi VFO yang “Rock Solid”. Beberapa kali browsing membawa saya kepada satu rangkaian VFO yang kemudian sesuai ilham yang saya terima dipadukan dengan buffer generik serta disusun dengan metode bodol pokoknya jadi dulu tidak peduli apa kata orang terhadap rangkaian tersebut.
Beginilah skema berdasarkan ilham yang saya dapat :





Selanjutnya saya buatkan PCB dengan rancangan awal akan menggunakan satu varco biasa. Namun demikian di tengah perjalanan proses saya menemukan sebuah benda eks tuner FM, semula saya kira sejenis varco tapi bentuknya berbeda tetapi ternyata benda itu adalah variabel inductor, yang apa boleh buat karena dia muncul ketemu saya akhirnya saya libatkan juga dalam rangkaian osilator ini.
Inilah si variabel inductor eks tuner FM tersebut :





Induktor ini mempunyai 6 silinder, 3 silinder kosong dan 3 silinder isi.  Silinder yang berisi lilitan terdapat masing-masing sepasang kawat email yang keluar di bagian bawahnya, semua saya hubungkan seri.  Nilai induktansi saya ukur antara 0,03 uH sampai 0,18 uH jika diputar kenopnya sampai pol bisa sekitar 5 – 7 putaran.

Setelah disolder maka dia jadi begini :




Dapat dilihat bahwa lay out PCB mengikuti gambar skema untuk memudahkan kontrol.  Kapasitor 1000 pF dua buah menggunakan polystyrene alias padder alias kapasitor kertas dan satu buah kapasitor NP0 500 pF.  Koil L1 pada koker 8 mm dipasang tanpa ferit untuk membantu kestabilan osilator.  Dalam eksperimen ini osilator belum dilakukan shielding.

HASIL  EKSPERIMEN :

1.  Jangkauan frekuensi didapat antara 2,450 MHz sampai dengan 3,100 MHz dengan tuning menggunakan varco.  Adapun tuning menggunakan PTO menghasilkan pergeseran frekuensi antara 40 – 50 kHz sehingga cocok digunakan sebagai Fine Tuning.  Pergeseran 40 – 50 kHz tersebut diperoleh dari 5 – 7 kali putaran.  Dengan jangkauan frekuensi seperti ini maka sangat cocok digunakan sebagai osilator lokal untuk transceiver BITX 40 m Band dengan IF 10 MHz, seperti yang akan saya buat berikutnya hehehe . . .
Variabel inductor ini boleh tidak dipasang, sebagai gantinya silahkan membuat rangkaian fine tuning dari varco kapasitas kecil (diseri dengan kapasitor 10 – 25 pF) atau menggunakan dioda/varactor.

2.  Apabila rangkaian resonansi menggunakan kapasitor NP0 (bukan varco) maka osilator lebih cepat stabil dibandingkan dengan jika menggunakan varco. Masalahnya adalah lebar tuning yang hanya berkisar 40 – 50 kHz menyebabkan kita harus menyediakan beberapa kapasitor untuk menjangkau lebar frekuensi yang diinginkan dan disusun berupa rangkaian menggunakan switch rotary atau cara lainnya.

3.  Kestabilan frekuensi sangat memuaskan, setelah stabil maka naik turun hanya pada satuan Hertz saja sehingga tidak perlu menggunakan rangkaian FLL lagi.

4.  Beberapa bagian rangkaian di atas disusun berlebih-lebihan antara lain pada datasheet dikatakan bahwa output dari NE602 merupakan “buffered output” tetapi tetap saya beri rangkaian buffer.  Demikian pula untuk regulasi tegangan sebetulnya cukup menggunakan satu buah IC 7805 tetapi saya pasang 7809 baru dilanjutkan 7805.  Tidak apa-apa, jika anda tetap mengikuti skema di atas berarti anda secara sukarela mengikuti kebodohan yang sudah saya perbuat dalam menerima ilham tentang rangkaian ini, mudah-mudahan anda ikhlas dan mendapat pahala yang setimpal.  Aamiiin.


Selamat bereksperimen, mudah-mudahan anda bisa menemukan IC NE602 / SA602 atau persamaannya yaitu NE612 atau SA612.

z

Posted in Uncategorized

13 Comments
Tags: NE602, SA602, stable VFO, VFO, VFO BITX

POS-POS TERBARU
Transistor CLASS E Exciter/Driver
Series Modulator TDA2050
ALBaN Antenna
Power Supply Linier
Linear Loaded EFHW Antenna
JAGAWANA

Tidak perlu mencari sesuatu yang sempurna. 
