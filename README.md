# Praktikum 3 web: Membuat List, Table dan Form

## Langkah-langkah Praktikum
-Persiapan membuat dokumen HTML dengan nama file lab3_list.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```

![Screenshot (1)](https://github.com/sayaveni04/lab3web/assets/115862597/4d2d9813-424d-43b8-a89e-4e10e05d6044)


### Membuat Ordered List
- Kemudian tambahkan kode untuk membuat Ordered List seperti berikut.
```
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
      <li>Pemrograman Web</li>
      <li>Sistem Informasi</li>
      <li>Basis Data 2</li>
    </ol>
</section>
```

![Screenshot (2)](https://github.com/sayaveni04/lab3web/assets/115862597/e8122149-062c-40de-95b4-4bb8a64a7391)


### Membuat Unorderd List
- Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada section unordered-list, seperti berikut.
```
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
      <li>Jaringan Komputer</li>
      <li>Struktur Data</li>
      <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```

![Screenshot (8)](https://github.com/sayaveni04/lab3web/assets/115862597/54df99e7-0904-4996-838f-8374ecfb7aa4)



### Membuat Description List
- Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.
```
<section id="unorder-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industi</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntasi</dd>
            <dd>Manajemen</dd>
            <dd>BisnIS Digital</dd>
        </dl>
    </section>
```

![Screenshot (4)](https://github.com/sayaveni04/lab3web/assets/115862597/733eff36-a707-451d-b583-c04ac351ea3f)




### Membuat Tabel
- Buat file baru dengan nama lab3_tabel.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>HTML lanjutan</title>
</head>
<body>
  <header>
    <h1>Membuat table</h1>
  </header>
</body>
</html>
```

- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```
<table border="1" cellpadding="4" cellspacing="3">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td>Teknik</td>
      <td>Teknik Informatika</td>
  </tr>
  <tr>
      <td>2.</td>
      <td>Teknik</td>
      <td>Teknik Industri</td>
  </tr>
  <tr>
      <td>3.</td>
      <td>Teknik</td>
      <td>Teknik Lingkungan</td>
  </tr>
  </tbody>
</table>
```

![Screenshot (5)](https://github.com/sayaveni04/lab3web/assets/115862597/039dd695-101a-4315-ae9c-62a4c7701d3a)


### Mengatur Margin dan Padding
- Untuk mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan cellspacing pada tag table.

```
<table border="1" cellpadding="4" cellspacing="3">
```

![Screenshot (9)](https://github.com/sayaveni04/lab3web/assets/115862597/3648848a-2926-4153-8f0c-cd98718e4127)



### Menggabungkan Sel Data
- Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara horizontal).
```
<table border="1" cellpadding="6" cellspacing="0">
  <thead>
    <tr>
      <th>No.</th>
      <th>Fakultas</th>
      <th>Program Studi</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1.</td>
      <td rowspan="3">Teknik</td>
      <td>Teknik Informatika</td>
  </tr>
  <tr>
      <td>2.</td>
      <td>Teknik Industri</td>
  </tr>
  <tr>
      <td>3.</td>
      <td>Teknik Lingkungan</td>
  </tr>
  </tbody>
</table>
```
![Screenshot (6)](https://github.com/sayaveni04/lab3web/assets/115862597/00551f5e-d7c2-4ba2-b07a-e4fd61a80651)


### Membuat Form
- Buat file baru dengan nama lab3_form.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>Membuat From</header>
</body>
</html>
```

- Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut.

```
form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
    <p>
        <label for="nama">Nama</label>
        <input type="text" id="nama" name="nama">
    </p>
    <p>
        <label for="alamat">Alamat</label>
        <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
    </p>
    <p>
        <label>Jenis Kelamin</label>
        <input id="jk_l" type="radio" name="kelamin" value="L" /><label
        for="jk_l">Laki-laki</label>
        <input id="jk_p" type="radio" name="kelamin" value="P" /><label
        for="jk_p">Perempuan</label>
    </p>
        <p><input type="submit" value="Login"></p>
        </fieldset>
</form>
```



### Menabahkan Style pada Form
- Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.
```
 <style>
        form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
```



### Pertanyaan dan Tugas
- Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.


