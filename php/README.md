# PHP

## Kenapa PHP?

- Relatif mudah untuk pemula
- Pre-requisite **HTML + CSS**
- Gratis dan open source
- Dukungan komunitas
- Dokumentasinya lengkap
- PHP dibuat khusus untuk web
- Kebanyakan website yang ada saat ini dibuat dengan PHP
- Banyak Content Management System yang menggunakan PHP
- Framework PHP

## Apa yang akan dipelajari?

- client-site vs server-side scripting
- static vs dynamic website
- persiapan lingkungan pengembangan
- sintaks PHP
- Array
- Request method
- Studi kasus website sederhana
- Database
- CRUD (create, read, update, delete)
- Login & registrasi
- Session & cookie
- Ajax
- Upload file
- Reporting
- Web hosting

## Karakteristik bahasa PHP

- Ekstensi file .php
- Ditulis di dalam tag php
  - delimiter
  - diawali dengan <?php
  - diakhiri dengan ?>
    
    ```php
    <?php
      echo "Hello World!";
    ?>
    ```
- bisa digunakan bersamaan dengan HTML
- mengikuti bahasa C

## Sintaks PHP

### Penulisan Sintaks PHP
1. PHP di dalam HTML
   ```php
   <h1><?php echo "PHP di dalam HTML"; ?></h1>
   <p>Halo, selamat datang <?php echo $nama; ?></p>
   ``` 
   
2. HTML di dalam PHP (tidak disarankan)
   ```php
   <?php 
     echo "<h1>HTML di dalam PHP</h1>";
   ?>
   ```

### Komentar
```php
// ini komentar

/*
  ini juga komentar
*/
```

### Standar Output
- echo
  ```php
  echo "Hello World!"; // Hello World!
  echo 123; // 123
  echo true; // 1
  echo false; // kosong
  ```
- print_r
  ```php
  print_r("Hello World!"); // Hello World!
  ```
- var_dump (untuk debugging)
  ```php
  var_dump("Hello World!"); // string(12) "Hello World!"
  ```
  
### Variable
Tidak boleh di awali dengan angka, tapi boleh mengandung angka

```php
$text = "Hello World!";
$x = 123;

$nama = "Kang Seul-gi";

// 👉 interpolasi
echo 'Halo, nama saya $nama'; // Halo, nama saya $nama
echo "Halo, nama saya $nama"; // Halo, nama saya Kang Seul-gi
```

### Operator
#### Aritmatika

```php
// 👉 + - * / %

echo 100 + 100; // 200

$x = 10;
$y = 20;
echo $x * $y; // 200
```

#### Penggabungan String / Concatenation / Concat

```php
// 👉 .

$nama_depan = "Bae";
$nama_belakang = "Joo hyun";
echo $nama_depan . " " . $nama_belakang; // Bae Joo hyun
```

#### Assignment

```php
// 👉 =, +=, -=, *=, /=, %=, .=

$i = 5;
$i -= 1;
echo $i; // 4

$name = "Kim";
$name .= " ";
$name .= "Ye-rim";
echo $name; // Kim Ye-rim
```

#### Perbandingan

```php
// 👉 <, >, <=, >=, ==

var_dump(1 == "1"); // bool(true)
```

#### Identitas

```php
// 👉 ===, !==

var_dump(1 === "1"); // bool(false)
```

#### Logika

```php
// 👉 &&, ||, !

$j = 10;
var_dump($j < 20 && $j % 2 == 0); // bool(true)
```




