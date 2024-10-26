# Lab 4 web

# Cara Membuat Box Element

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
  <header>
    <h1>Box Element</h1>
  </header>
</body>
</html>
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
</section>
```
## CSS element box

```css
<style>
  div {
    float:left;
    padding: 10px;
  }
  .div1 {
    background: red;
  }
  .div2 {
    background: yellow;
  }
  .div3 {
    background: green;
  }
</style>
```
## Hasil Dari Code Diatas

![Screenshot 2024-10-25 074606](https://github.com/user-attachments/assets/93a20996-5b20-4c32-84c8-56dc76edc9d9)

# Mengatur Clearfix Element

```html
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">Div 4</div>
</section>
```

## CSS Clearfix Element

```css
.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```
# Hasil Dari Code Diatas
![Screenshot 2024-10-25 075307](https://github.com/user-attachments/assets/362a6f9a-7316-4156-9e57-ec0b3712bcbb)

# Membuat Layout Sederhana

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">

    </div>
</body>
</html>
```

```html
<header>
    <h1>Layout Sederhana</h1>
</header>
<nav>
    <a href="home.html" class="active">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html">Kontak</a>
</nav>
<section id="hero"></section>
<section id="wrapper">
    <section id="main"></section>
    <aside id="sidebar"></aside>
</section>
<footer>
    <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

## Hasil Dari Code Diatas
![Screenshot 2024-10-25 075609](https://github.com/user-attachments/assets/4dd8aedd-515d-431a-9854-60b1dd313ad4)

## CSS
```css
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400
;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0
,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
    margin: 0;
    padding: 0;
}

body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}

#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

/* header */
header {
    padding: 20px;
}

header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```

## Hasil Dengan CSS
![Screenshot 2024-10-25 075644](https://github.com/user-attachments/assets/55dabe5a-d45c-48fd-9fa6-2a46e9af2444)


# Membuat Navigasi
```css
/* navigasi */
nav {
    display: block;
    background-color: #1f5faa;
}
nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}
nav a.active,
nav a:hover {
    background-color: #2b83ea;
}
```
## Hasil Dari Code Diatas
![Screenshot 2024-10-25 075713](https://github.com/user-attachments/assets/c44e9482-bb41-4cf6-bb1e-531c56a5e451)


# Membuat Hero Panel
```html
<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
```css
/* Hero Panel */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1 {
    margin-bottom: 20px;
    font-size: 35px;
}
#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}
```

## Hasil Dari Code Diatas
![Screenshot 2024-10-25 075754](https://github.com/user-attachments/assets/9815097a-14d3-4153-903b-76a18f320c90)


## Mengatur Layout & Sidebar
```css
/* main content */
#wrapper {
    margin: 0;
}
#main {
    float: left;
    width: 640px;
    padding: 20px;
}
/* sidebar area */
#sidebar {
    float: left;
    width: 260px;
    padding: 20px;
}
```
```html
<aside id="sidebar">
    <div class="widget-box">
        <h3 class="title">Widget Header</h3>
        <ul>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
            <li><a href="#">Widget Link</a></li>
        </ul>
    </div>
    <div class="widget-box">
        <h3 class="title">Widget Text</h3>
<p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
pharetra est nunc, nec pretium nunc pretium ac.</p>
    </div>
</aside>
```
<h1>Kemudian Tambahkan CSS</h1>

```css
/* widget */
.widget-box {
    border:1px solid #eee;
    margin-bottom:20px;
}
.widget-box .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff;
}

.widget-box ul {
    list-style-type:none;
}

.widget-box li {
    border-bottom:1px solid #eee;
}

.widget-box li a {
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none;
}
.widget-box li:hover a {
    background-color:#eee;
}
.widget-box p {
    padding:15px;
    line-height:25px;
}
```
## Hasil Dari Code Diatas
![Screenshot 2024-10-25 075830](https://github.com/user-attachments/assets/b32d07eb-e062-4f2a-9855-293997649672)

# Mengatur Footer
```css
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
```
## Hasil Dari Code Diatas
![Screenshot 2024-10-25 082210](https://github.com/user-attachments/assets/cee724d8-5d08-42df-9edf-5f103ada9896)

## Menambahkan Element Lainnya Pada Main Content
```html
<section id="main">
    <div class="row">
        <div class="box">
            <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
        </div>
        <div class="box">
            <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
class="image-circle">
            <h3>Heading</h3>
            <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
            <a href="#" class="btn btn-default">View detail</a>
        </div>
        <div class="box">
            <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
        <h3>Heading</h3>
        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
euismod.</p>
        <a href="#" class="btn btn-default">View detail</a>
        </div>
    </div>
</section>
```
## CSS
```css
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
    padding:0 10px;
    text-align:center;
}

.box h3 {
    margin: 15px 0;
}

.box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px;
}

.box img {
    border: 0;
    vertical-align: middle;
}

.image-circle {
border-radius: 50%;
}

.row {
    margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box;
}

.row:after, .row:before,
.entry:after, .entry:before {
    content:'';
    display:table;
}

.row:after,
.entry:after {
    clear:both;
}
```

## Hasil Dari Code Diatas
![Screenshot 2024-10-25 075909](https://github.com/user-attachments/assets/acd6ad6d-5631-4539-8615-e9fe06a759d8)

# Menambahkan Content Artikel
```html
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
</article>
```
```css
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0;
}

/* entry */
.entry {
    margin: 15px 0;
}

.entry h2 {
    margin-bottom: 20px;
}

.entry p {
    line-height: 25px;
}

.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
}

.entry .right-img {
    float: right;
}
```

## Hasil Dari Code Diatas
![Screenshot 2024-10-25 075937](https://github.com/user-attachments/assets/45196043-bd7c-41d1-a3da-5132013e16d9)

# Tugas Membuat Layout About & Kontak

## Menu About

```html
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>About Me</h1>
        </header>
        <nav>
            <a href="home.html">Home</a>
            <a href="about.html" class="active">About</a>
            <a href="artikel.html">Artikel</a>
            <a href="kontak.html">Kontak</a>
        </nav>
        <section id="main">
            <h2>Deskripsi</h2>
            <p>Adira Alvian Zein</p>
            
            <h2>Portfolio</h2>
            <p>TI.23.A3 Web Designer</p>
        </section>
        <footer>
            <p>&copy; 2021 - Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```

## Menu Kontak
```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kontak Kami</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Contact Us</h1>
        </header>
        <nav>
            <a href="home.html">Home</a>
            <a href="about.html">About</a>
            <a href="artikel.html">Artikel</a>
            <a href="kontak.html" class="active">Kontak</a>
        </nav>
    <h1>Kontak Kami</h1>

    <p>Jika Anda memiliki pertanyaan atau ingin menghubungi kami, silakan isi formulir di bawah ini:</p>

    <form action="/submit_form" method="post">
        
        <label for="name">Nama:</label><br>
        <input type="text" id="name" name="name" required><br><br>

        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email" required><br><br>

        <label for="phone">Nomor Telepon:</label><br>
        <input type="tel" id="phone" name="phone"><br><br>

        <label for="message">Pesan:</label><br>
        <textarea id="message" name="message" rows="4" required></textarea><br><br>

        <input type="submit" value="Kirim">
    </form>

    <p>Atau hubungi kami melalui:</p>
    <ul>
        <li>Email: Universitas Pelita Bangsa</li>
        <li>Telepon: 021 2851 8181,82,83,84</li>
        <li>Alamat: Jl.Inspeksi Kalimalang Tegal Danas Arah Deltamas, Cibatu, Cikarang</li>
    </ul>

</body>
</html>
```







