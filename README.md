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
# CSS element box

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
# Hasil Dari Code Diatas

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

# CSS

```css
.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```
# Hasil Dari Code Diatas


