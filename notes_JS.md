# Catatan untuk JS atau ECMAscript dan lainnya yang berhubungan

## Array Method

```javascript
// variabel buah
let buah = ['jambu','apel','mangga','duren','sukun','jeruk','anggur','salak'];
```

```javascript
// array ke string
buah.toString();
// hasil : jambu,apel,mangga,duren,sukun,jeruk,anggur,salak
```

```javascript
// tambah elemen dari belakang array
buah.push('nanas');
console.log(buah); 
/* hasil : 
 ['jambu',  'apel',
  'mangga', 'duren',
  'sukun',  'jeruk',
  'anggur', 'salak',
  'nanas']
  */
```
```javascript
// hapus elemen dari belakang array
// ga perlu diisi parameter
buah.pop();
console.log(buah); 
/* hasil : 
['jambu',  'apel',
  'mangga', 'duren',
  'sukun',  'jeruk',
  'anggur']
  */
```

```javascript
// cek array apakah mengandung elemen tertentu
buah.includes('pisang'); 
// hasil : false
// elemen pisang tidak ada di array buah
```
```javascript
// cek indeks suatu element
buah.indexOf('pisang');
// hasil : 0
// indeks pada array JS dimulai dari 0
// indeks bernilai -1 jika elemen tidak ada dalam array
```

```javascript
// menggabungkan elemen pada array dengan string tertentu
buah.join('-');
// hasil : jambu-apel-mangga-duren-sukun-jeruk-anggur-salak
```

```javascript
// mengambil element tertentu dari array
buah.slice(1,3);
// hasil : [ 'apel', 'mangga' ]
// parameter -> ambil elemen dari array 1 sampai dengan sebelum array 3
// elemen 1 : apel
// elemen sebelum 3 : mangga
```
```javascript
// method ajaib yang bisa digunakan utk hapus, tambah, ganti element
// formula : array.splice(index, jumlahDelete, value1,value2,...)

// hapus elemen
console.log(buah.splice(0,2)); // hasil: [ 'jambu', 'apel' ]
console.log(buah); // hasil : [ 'mangga', 'duren', 'sukun', 'jeruk', 'anggur', 'salak' ]

// tambah 1 element pada indeks 0
buah.splice(0,0,'extrajoss'); // dari indeks-0 dihapus 0 element, item 'extrajoss'
console.log(buah);
// hasil : 
/*
[
  'extrajoss', 'jambu',
  'apel',      'mangga',
  'duren',     'sukun',
  'jeruk',     'anggur',
  'salak'
]
*/
// ganti elemen sukun jadi kwaci
buah.splice(4,1,'kwaci');
console.log(buah);
/* hasil
[
  'jambu',  'apel',
  'mangga', 'duren',
  'kwaci',  'jeruk',
  'anggur', 'salak'
]

*/

```

nb : belum selesai, masih ada objek method dll di ig yang blm slseai di masukkan di catatan

## Arrow function

Arrow functions biasanya dipakai untuk  callback functions or anonymous functions karena lebih enak dibaca.
Arrow function lebih enak lagi saat dipake dengan higher-order functions seperti map, filter, or reduce.

