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

### Control Flow / Struktur Kendali
#### Pengulangan
- for
  ```php
  for ($i = 0; $i < 5; $i++) {
    echo "'For' loop $i <br />";
  }
  ```
- while
  ```php
  $i = 0;
  while($i < 5) {
    echo "'While' loop $i <br />";
    $j++;
  }
  ```
- do.. while
  ```php
  $i = 0;
  do {
    echo "'do.. while' loop $i <br />";
    $i++;
  } while ($i < 5);
  ```
- foreach (pengulangan khusus array)
  
#### Pengkondisian
- if.. else
  ```php
  $x = 23;
  if($x < 20) {
    echo "true";
  } else {
    echo "false";
  }
  ```
- if.. else if.. else
  ```php
  $x = 20;
  if($x < 20) {
    echo "true";
  } else if($x == 20) {
    echo "bingo";
  } else {
    echo "false";
  }
  ```
- ternary
- switch

**Contoh penggunaan 'for'**
```php
<table border="1" cellpadding="10" cellspacing="0">
  <?php 
    for ($i = 1; $i <= 3; $i++) {
      echo "<tr>";
      for ($j = 1; $j <=5; $j++) {
        echo "<td>$i,$j</td>";
      }
      echo "</tr>";
    }
  ?>
</table>

// 👉 menggunakan sintaks templating
<table border="1" cellpadding="10" cellspacing="0">
  <?php for($i = 1; $i <= 3; $i++) : ?>
    <tr>
      <?php for($j = 1; $j <= 5; $j++) : ?>
        <td><?php echo "$i, $j"; ?></td>
      <?php endfor; ?>
    </tr>
  <?php endfor; ?>
</table>
```
![image](https://github.com/fnurrahmah125/wpu_fullstack/assets/54012198/2737408b-4c8f-4830-ae6d-69c5e1a3e5c3)


**Contoh penggunaan 'if.. else'**
```php
<table border="1" cellpadding="10" cellspacing="0">
  <?php for($i = 1; $i <= 5; $i++) : ?>
    <?php if($i % 2 == 1) : ?>
      <tr class="warna-baris">
    <?php else : ?>
      <tr>
    <?php endif; ?>
      <?php for($j = 1; $j <= 5; $j++) : ?>
        <td><?php echo "$i, $j"; ?></td>
      <?php endfor; ?>
    </tr>
  <?php endfor; ?>
</table>
```
![image](https://github.com/fnurrahmah125/wpu_fullstack/assets/54012198/86667e3f-134c-481c-96eb-ecd74b865e63)

