# Belajar-JavaScript

### Synchronous dan Asynchronous
Dalam dunia programming istilah tersebut diguakan untuk membedakan cara mengeksekusi perintah dalam kodingan.

- **Synchronous** adalah cara mengeksekusi kode dengan cara mengurutkan.
Contoh:

```
console.log('Hello')
console.log('Javascript')
console.log('Coder')

/*
Output :
Hello!
Javascipt
Coder
*/
```

Output dari kode diatas dijalankan dengan sesusai urutan, perintah kode tersebut dapat dijalankan setelah perintah sebelumnya selesai. Hal ini dapat disebut sebagai proses **Synchronous** atau teknik **blocking**.

- **Asynchronous** adalah cara mengekseskusi kode yang memiliki output yang tidak berdasarkan sesuai urutan kode , tetapi berdasarkan waktu proses.
Contoh:

```
console.log('Hello');
setTimeout(() => { console.log('Javascript')},100) // tunda selama 100 miliseconds
console.log('Coder');

/* ----------
Output :
Hello!
Coder
Javascipt
------------*/
```

Output dari kode diatas memiliki output yang tidak berutuan, kaena pada baris ke 2 memakai fungsi `setTimeout` yang digunakan untuk menunda eksekusi, dalam hal ini untuk simulasi proses async.

Hal tersebut dapat kita tarik kesimpulan bahwa proses tersebut tidak saling menunggu, sembari mengunggu waktu proses javascript mengeksekusi perintah berikutnya. Hal ini dapat disebut sebagai proses **Asyncronous** atau teknik **Non Blocking**.





















