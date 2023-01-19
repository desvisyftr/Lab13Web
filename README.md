# Lab13Web

## Membuat Pagination
Pagination digunakan untuk membatasi atau membagi record data yang akan ditampilkan pada
laman web. Dari seluruh record data yang ada akan dibagi berdasarkan jumlah record
per-halaman. Pada prinsipnya untuk membatasi tampilan record data pada query mysql menggunakan LIMIT dan OFFSET;
Query alwal:
$sql = `SELECT * FROM tabel_barang`;
Untuk menapilkan data dari record ke 1 sampai record ke 10:
$sql = `SELECT * FROM table_barang LIMIT 10`;
Untuk menampilkan data dari receord ke 11 sampai dengan record ke 20, disini digunakan
OFFSET:
$sql = `SELECT * FROM table_barang LIMIT 10,20`;
Untuk membagi jumlah halaman, tentu kita harus ketahui dulu jumlam record secara keseluruhan,
selanjutnya di bagi dengan jumlah record per halaman, maka akan diketahui jumlah halamannya.

![img]screenshot/ss.png