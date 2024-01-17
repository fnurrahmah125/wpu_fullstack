# HTML

Hypertext Markup Language. Digunakan untuk menyajikan konten dan struktur dari halaman.

**Referensi:**
- www.w3.org
- www.evolutionoftheweb.com

## Tag pada HTML

Tag yang bisa disimpan di bagian `<head></head>`
- Judul halaman
  
  `<title></title>`
- CSS

  `<style></style>`
- JavaScript

  `<script></script>`
- Metadata

  `<meta></meta>`

Tag yang bisa disimpan di body `<body></body>`
- Teks

  `<h1> <h2> <h3> <h4> <h5> <h6> <p> ...`
- Pendukung teks

  `<br> <hr> <em> <strong>`
- Gambar

  `<img>`
- Hyperlink

  `<a>`
- List (bullets & numbering)

  `<ul> <ol> <li> <dl> <dt> <dd>`
- Tabel

  `<table> <thead> <tbody>`
- Form

  `<form> <input> <select> <button>`
- Script

  `<script>`
- Object

  `<object>`
- Grouping

  `<div><span>`
- Comment

  `<!--- --->`

## Struktur Tag

![image](https://github.com/fnurrahmah125/wpu_html/assets/54012198/81d803f2-fe88-46ca-8ace-0fab037b6385)

Boleh tidak mempunyai atribut atau mempunyai atribut lebih dari satu.

## Atribut Global

accesskey, class, id, dir, lang, style, tabindex, title

## Paragraf

- `<p>` : menuliskan paragraf
- `<br>` : menambahkan baris baru
- `<hr>` : membuat garis horizontal
- `<b></b>` : bold
- `<i></i>` : italic
- `<u></u>` : underline
- `<em></em>` : penekanan pada sebuah teks
- `<strong></strong>` : penekanan lebih pada sebuah teks

## Heading

Heading 1 lebih penting dari heading-heading di bawahnya.

``` html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```

## List

- `<ol></ol>` : untuk membuat list terurut (ordered list)
  
  ``` html
  <ol>
    <li>item 1</li>
    <li>item 2</li>
  </ol>

  <ol type="1"></ol>
  <ol type="A"></ol>
  <ol type="a"></ol>
  <ol type="I"></ol>
  <ol type="i"></ol>
  ```
- `<ul></ul>` : untuk membuat list tidak terurut (unorder list)

   ``` html
  <ul type="disc"></ul>  
  <ul type="square"></ul>  
  <ul type="circle"></ul>  
  ```
- `<dl></dl>` : untuk membuat daftar definisi atau terminologi (definition list)
   ``` html
  <dl>
    <dt><strong>HTML</strong></dt>
    <dd>Hypertext Markup Language</dd>
    <dt><strong>CSS</strong></dt>
    <dd>Cascading Style Sheet</dd>
  </dl>
  ```
  
## Hyperlink

`<a href=""></a>` anchor

- External link
  
  `https://www.google.com/`
  
  `https://twitter.com/`
  
- Internal link / Relative Url

  `product.html`
  
  `../admin/index.html`
  
- Page anchor

  `#about`

  `index.html#contact`
  
- Target

  `<a href="user/halaman1.html" target="_blank">Halaman 1</a>`
  
  `<a href="user/halaman1.html" target="_self">Halaman 1</a>`
  
  `<a href="user/halaman1.html" target="_parent">Halaman 1</a>`
  
  `<a href="user/halaman1.html" target="_top">Halaman 1</a>`

## Image

- Internal resource

  `<img src="images/logo.png">`
  
- External resource / hotlink (tidak disarankan)

  `<img src="https://unsplash.it/640/425">`
  
- Attribute dan value pada tag `<img>`
  
  `<img src="" alt="" title="" width="" height="">`
  
  Untuk **width** dan **height** jika ditulis angka saja maka ukurannya akan berbentuk pixel, jika ditambah persen (%) maka ukurannya akan relative terhadap halamannya.

- Hyperlink + image

  ```html
  <a href="https://google.com/">
    <img src="image-1.jpg">
  </a>
  ```
















