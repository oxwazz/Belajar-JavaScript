# Belajar-JavaScript

### Synchronous dan Asynchronous
Dalam dunia programming istilah tersebut digunakan untuk membedakan cara mengeksekusi perintah dalam kode.

1. **Synchronous** adalah cara mengeksekusi kode dengan cara mengurutkan.
Contoh:

```
console.log('Hello')
console.log('Javascript')
console.log('Coder')

/*----------
Output :
Hello!
Javascipt
Coder
----------*/
```

Output dari kode diatas dijalankan dengan sesusai urutan, perintah kode tersebut dapat dijalankan setelah perintah sebelumnya selesai. Hal ini dapat disebut sebagai proses **Synchronous** atau teknik **blocking**.

2. **Asynchronous** adalah cara mengekseskusi kode yang memiliki output yang tidak berdasarkan sesuai urutan kode , tetapi berdasarkan waktu proses.
Contoh:

```
console.log('Hello');
setTimeout(() => { console.log('Javascript') }, 100) // tunda selama 100 miliseconds
console.log('Coder');

/*----------
Output :
Hello!
Coder
Javascipt
------------*/
```

Output dari kode diatas memiliki output yang tidak berutuan, kaena pada baris ke 2 memakai fungsi `setTimeout` yang digunakan untuk menunda eksekusi, dalam hal ini untuk simulasi proses async.

Hal tersebut dapat kita tarik kesimpulan bahwa proses tersebut tidak saling menunggu, sembari mengunggu waktu proses javascript mengeksekusi perintah berikutnya. Hal ini dapat disebut sebagai proses **Asyncronous** atau teknik **Non Blocking**.

### Pertanyaan Synchronous dan Asynchronous
1. Secara default metode apa yang dipakai javascript dalam mengkesekusi perintah?
2. Bisakah kita membuat proses asynchronous ?
3. Dalam kasus apa teknik asynchronous digunakan ?

**Jawabannya**
1. Javascript secara default mengeksekusi perintah secara synchronous, kecuali untuk beberapa hal seperti : ajax,websocket, worker, file, database, animasi dan beberapa hal lainya.
2. Kita tidak bisa membuat proses asynchronous murni. Tapi untuk membuat simulasi iya kita bisa menggunakan fungsi setInternal dan setTimeout
3. Teknik Asynchronous paling banyak digunakan mengelola komunikasi yang tidak mungkin sinkron atau harus menunggu seperti proses request ajax, operasi file, koneksi ke database, websocket, real time communication seperti pada aplikasi chating dan masih banyak lagi.

sumber: https://medium.com/coderupa/panduan-komplit-asynchronous-programming-pada-javascript-part-1-fca22279c056



















