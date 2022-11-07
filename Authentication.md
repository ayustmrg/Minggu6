# Authentication & Authorization in Express  

### Authentication
autrorization nanya kamu punya izin apa, punya wewenang apa  
data user semisal hanya bisadicek admin  
kalau ada izinkan data, kalau engga maka ngasih status code 403 dan message  
login make method post
berusaha mengenali, dan datanya ada maka dikasih token  

</br>

### Authorization  
nanya dia punya hak apa, semisal dia dmin, maka dia bisa mengakses data si user  

</br>

<img src="au1.jpeg" width="200" height="100">  

<img src="au2.jpeg" width="200" height="100">  

<img src="au3.jpeg" width="200" height="100">  

token itu tanda pengenal, isinya cuman id user (brda2 tiap org)  

token dibawa kembali ke login, fe akan menyimpan di local storarge  

ketika mengakses end point sekalian kirim data  

<img src="au4.jpeg" width="200" height="100">   

>maka akan ditangkap disini  

<img src="au5.jpeg" width="200" height="100">  

>untuk movies nya  

<img src="au6.jpeg" width="200" height="100">   

<img src="au7.jpeg" width="200" height="100">  

>setelah diset up maka akan ada

<img src="au8.jpeg" width="200" height="100">  

>datanya dr sini

<img src="au9.jpeg" width="200" height="100">  

>berhasil req data dr body  

sekarang ngecek apakah email dan pass nya bener  

selanjutnya dimanipulasi

<img src="au10.jpeg" width="200" height="100">  

>dengan cara

<img src="au11.jpeg" width="200" height="100">  

>apakah ini

<img src="au12.jpeg" width="200" height="100">  

>sama dengan ini, fungsi code tdi

<img src="au13.jpeg" width="200" height="100">  

>membuat return  

<img src="au14.jpeg" width="200" height="100">  

>hasilnya, berhasil

<img src="au15.jpeg" width="200" height="100">  

>cth dia memeriksa email dan pass nya

<img src="au16.jpeg" width="200" height="100"> 

>bisa juga make rest

<img src="au17.jpeg" width="200" height="100"> 

>setiap mau ngirim data dan tambah data make method post

</br>

<img src="au18.jpeg" width="200" height="100">  

>enkripsi, ubah bahasa formal ke bahasa sendri

<img src="au19.jpeg" width="200" height="100"> 

>pengertian enkripsi

<img src="au20.jpeg" width="200" height="100">  

<img src="au21.jpeg" width="200" height="100"> 

>bedanya :encryption acak atau beda cara  
encryption bisa buat jd kata2 susah, bisa dibalikin dgn algoritma yg sama, cara yg sama  
hashing : ngacakin, beneran diacak, dibuatin format, ke format teks random  
hasing ada tambahan salt

<img src="au22.jpeg" width="200" height="100">  

>contoh hasing  
pass ditambah satu kata2 unik, satu kumpulan yg unik yg bisa berubah2

<img src="au23.jpeg" width="200" height="100">  

>cth penggunaan hasing  
ketika ada pass yg sama maka encrypt nya sama, makanya susah digunakan  
jdi semisal nih dia make email ke 3 tp luap angka 2, dia berhasil masuk kalau make encrypt maka berhasil masuk, makanya make hasing agar dilakukan perbedaan  

</br>

token itu tanda penegnal, dengan bantuan jwt  
jwt ada masa expired nya, tokennya ada masa expired nya  
token itu gunanya biar siapapun yg melihat gk langsung liat datanya
