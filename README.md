# Tableau-Clustering

## A. Tableau 
- Tableau adalah
- drag & drop

### A.1 Clustering di Tableau
- Clustering adalah
Dengan cara sebagai berikut :
- 1.) Masukkan filenya

###1

Menuju ke lembar kerja
###1.2

- 2.) Variabel/acuannya 
drag Measures variabel1 drop ke columns > drag Measures variabel2 drop ke rows > drag Dimensions variabel3 drop ke Marks Detail > muncul/tampil dalam bentuk scatter chart

###2
###2.2 tambahan drag variabel

- 3.) Melakukan Clustering
klik analytics > pada Model pilih & drag cluster drop ke box cluster yang disediakan di lembar kerja

###3

muncul jendela baru untuk mengatur jumlah cluster
###3.2 muncul jendela baru untuk mengatur jumlah cluster

- 4) Mengubah format number 

###4
###4.2

- 5) Melihat cara pembagian clusternya 
di Marks klik tanda panah kebawah cluster > pilih/klik Describe clusters... > muncul jendela baru

Memperpanjang Chart 
###5
###5.2

di jendela baru tersebut/describe cluster kita dapat mengetahui informasi tentang:
- variables yang digunakan
- level of detailnya   : jadi setiap bulatan di chart tersebut mencerminkan/menggunakan variabel apa
- scaling normalized   : scalingnya di Tableau menggunakan min max scaller 

number of clusters     : ada berapa cluster
number of points       : jumlah data/bulatan di chart
beetwen-group sum of squares (jarak antar centroid per cluster)(semakin besar angkanya menunjukkan setiap cluster semakin berbeda) : clusteringnya berdasarkan k-means jadi terbentuk centroid-centroid
within-group sum of squares (jarak antar bulatan-bulatan dalam satu cluster)(semakin kecil angkanya menunjukkan setiap buletan dalam 1 cluster tersebut semakin serupa)
total sum of squares : hasil penjumlahan dari beetwen-group sum of squares dengan within-group sum of squares

informasi apa yang menyebabkan bulatan/data tersebut ada/masuk pada cluster tersebut, 
number of items : jumlah data/bulatan yang ada di cluster tersebut
not clustered : data yang tidak masuk di cluster manapun 

klik centang show scaled centres : untuk agar centresnya di scaled (angkanya berbentuk scales)


Kemudian klik models di jendela

###5.3

modelnya tergantung dari variabel-variabel yang dipakai/digunakan dalam clustering 

makin besar F-statistic berarti variabel semakin berbeda antar clusternya  (*antar variabel)
p-value kemungkinan angkanya lebih besar dari populasi cluster tersebut (makin kecil p-valuenya makin mirip dengan elemen-elemen yang ada di cluster tersebut) 

model : jika mean(rata-rata) antar clusternya dekat berarti valeunya jadi kecil***
seberapa deket si centernya*** 

jika ingin mengetahui lebih dalam klik "Learn more..."

- 6.0) Menampilkan beberapa cluster saja

###6

Mengubah warna cluster

###6.2
###6.3 tampilan terakhir chart

Melihat data dalam bentuk tabel

###7
###7.2

