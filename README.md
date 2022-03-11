# Tableau-Clustering

## A. Tableau 
- Tableau adalah aplikasi untuk visualisasi, mempelajari, dan mempresentasikan data.
- drag & drop

### A.1 Clustering di Tableau
- Clustering adalah pengelompokkan sesuatu yang lebih kecil berdasarkan adanya kemiripan satu sama lain.
- Lebih dalam akses: https://help.tableau.com/current/pro/desktop/en-us/clustering.htm 

Dengan cara sebagai berikut :
- 1.) Masukkan filenya

###
![1](https://user-images.githubusercontent.com/86678205/157829027-b4c3e7f9-df6c-4a16-8c7c-13f5794fa726.PNG)

Menuju ke lembar kerja/worksheet

###
![1 2](https://user-images.githubusercontent.com/86678205/157829137-a407ee1f-9534-4e6b-8c0c-a983999f21e9.PNG)

- 2.) Variabel/acuannya 
drag Measures variabel1 drop ke columns > drag Measures variabel2 drop ke rows > drag Dimensions variabel3 drop ke Marks Detail > muncul/tampil dalam bentuk scatter chart

###
![2](https://user-images.githubusercontent.com/86678205/157829482-d2c18ffc-2732-4581-a11b-c2c85abd1dd6.PNG)

Menambah variabel > Klik jendela analytics
###
![2 2](https://user-images.githubusercontent.com/86678205/157829648-f663d72c-cd3d-40b6-8386-927877977471.PNG)

- 3.) Melakukan Clustering
klik analytics > pada Model pilih & drag cluster drop ke box cluster yang disediakan di lembar kerja

###
![3](https://user-images.githubusercontent.com/86678205/157829797-29593554-851a-45a3-9bab-25099e304b42.PNG)

Muncul jendela baru untuk mengatur jumlah cluster

###
![3 2](https://user-images.githubusercontent.com/86678205/157829907-eaa83d29-0d96-40d4-8b6c-f1ca6d3b2cee.PNG)

- 4.) Mengubah format number 

###
![4](https://user-images.githubusercontent.com/86678205/157830166-6258365c-8aa2-4d5e-bfa9-2b6c44a370fd.PNG)

###
![4 2](https://user-images.githubusercontent.com/86678205/157830202-8342aec7-0713-472b-a9db-d5eeb1119df5.PNG)

- 5.) Melihat cara pembagian clusternya 
Pada Marks klik tanda panah kebawah cluster > pilih/klik Describe clusters... > muncul jendela baru

Panjangkan Chart 
###
![5](https://user-images.githubusercontent.com/86678205/157830335-699288b4-4725-4444-96e6-6e21426366b9.PNG)

###
![5 2](https://user-images.githubusercontent.com/86678205/157830357-e92098ea-6c03-4f85-9af4-095c58530158.PNG)

Pada jendela baru tersebut/describe cluster kita dapat mengetahui informasi tentang:
- variables yang digunakan
- level of detailnya   : jadi setiap bulatan di chart tersebut mencerminkan/menggunakan variabel apa
- scaling normalized   : scalingnya di Tableau menggunakan min max scaller 

- number of clusters     : ada berapa cluster
- number of points       : jumlah data/bulatan di chart
- beetwen-group sum of squares (jarak antar centroid per cluster)(semakin besar angkanya menunjukkan setiap cluster semakin berbeda) : clusteringnya berdasarkan k-means jadi terbentuk centroid-centroid
- within-group sum of squares (jarak antar bulatan-bulatan dalam satu cluster)(semakin kecil angkanya menunjukkan setiap buletan dalam 1 cluster tersebut semakin serupa)
- total sum of squares : hasil penjumlahan dari beetwen-group sum of squares dengan within-group sum of squares

- informasi apa yang menyebabkan bulatan/data tersebut ada/masuk pada cluster tersebut, 
- number of items : jumlah data/bulatan yang ada di cluster tersebut
- not clustered : data yang tidak masuk di cluster manapun 
- klik centang show scaled centres : untuk agar centresnya di scaled (angkanya berbentuk scales)

Kemudian klik models di jendela

###
![5 3](https://user-images.githubusercontent.com/86678205/157830412-88e28392-ae35-4379-bc9e-b558fdf65698.PNG)

- modelnya tergantung dari variabel-variabel yang dipakai/digunakan dalam clustering 
- makin besar F-statistic berarti variabel semakin berbeda antar clusternya  (*antar variabel)
- p-value kemungkinan angkanya lebih besar dari populasi cluster tersebut (makin kecil p-valuenya makin mirip dengan elemen-elemen yang ada di cluster tersebut) 
- model : jika mean(rata-rata) antar clusternya dekat berarti valeunya jadi kecil*** seberapa deket si centernya*** 
- jika ingin mengetahui lebih dalam klik "Learn more..."

- 6.) Menampilkan beberapa cluster saja

###
![6](https://user-images.githubusercontent.com/86678205/157830495-2b054eb7-8b2a-494e-8229-57d2d58e0f8b.PNG)

Mengubah warna cluster

###
![6 2](https://user-images.githubusercontent.com/86678205/157830530-7434c1d8-4d52-4069-8b94-bae01295acad.PNG)

Tampilan chart
###
![6 3](https://user-images.githubusercontent.com/86678205/157830576-358a74df-f696-497a-9aa8-92709f3c7967.PNG)

Melihat data dalam bentuk tabel

###
![7](https://user-images.githubusercontent.com/86678205/157830921-31d1a53d-fa49-4b4a-93a9-92e2e5e16f3f.PNG)

###
![7 2](https://user-images.githubusercontent.com/86678205/157830946-14876484-427a-459f-ae1d-775c233b735b.PNG)


