# BRELYSS.github.io
<html lang="pl"><head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Breloki Samochodowe - Sklep</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #111;
      color: #fff;
    }
    header {
      background-color: #000;
      padding: 20px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 2em;
      color: #e60000;
    }
    nav {
      display: flex;
      justify-content: center;
      gap: 20px;
      padding: 10px;
      background-color: #1a1a1a;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      cursor: pointer;
    }
    nav a:hover {
      color: #e60000;
    }
    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      padding: 20px;
    }
    .product {
      background-color: #1a1a1a;
      border: 1px solid #333;
      border-radius: 10px;
      margin: 15px;
      width: 280px;
      padding: 15px;
      text-align: center;
      transition: transform 0.2s;
    }
    .product:hover {
      transform: scale(1.03);
    }
    .product img {
      width: 100%;
      height: auto;
      border-radius: 8px;
    }
    .product h2 {
      font-size: 1.3em;
      margin: 10px 0;
    }
    .product p {
      color: #ccc;
    }
    .price {
      color: #e60000;
      font-size: 1.2em;
      margin: 10px 0;
    }
    .btn {
      background-color: #e60000;
      border: none;
      color: white;
      padding: 10px 20px;
      font-size: 1em;
      border-radius: 5px;
      cursor: pointer;
    }
    .btn:hover {
      background-color: #cc0000;
    }
    footer {
      background-color: #000;
      text-align: center;
      padding: 15px;
      color: #777;
    }
  </style>
  <script>
    document.addEventListener('DOMContentLoaded', function () {
      const navLinks = document.querySelectorAll('nav a');
      const products = document.querySelectorAll('.product');

      navLinks.forEach(link => {
        link.addEventListener('click', function (e) {
          e.preventDefault();
          const brand = this.textContent.trim().toLowerCase();

          products.forEach(product => {
            const title = product.querySelector('h2').textContent.toLowerCase();
            if (title.includes(brand)) {
              product.style.display = 'block';
            } else {
              product.style.display = 'none';
            }
          });
        });
      });
    });
  </script>
<style type="text/css" id="operaUserStyle"></style></head>
<body>
  <header>
    <h1>Breloki Samochodowe</h1>
    <p>Styl, jakość i pasja motoryzacyjna</p>
  </header>

  <nav>
    <a href="#">Dodge</a>
    <a href="#">BMW</a>
    <a href="#">Audi</a>
    <a href="#">Mercedes</a>
    <a href="#">Toyota</a>
  </nav>

  <div class="container">
    <div class="product">
      <img src="https://example.com/brelok_dodge.jpg" alt="Brelok Dodge Premium">
      <h2>Brelok Dodge Premium</h2>
      <p>Skórzany brelok z metalowym wykończeniem</p>
      <p class="price">29,99 zł</p>
      <button class="btn">Dodaj do koszyka</button>
    </div>

    <div class="product">
      <img src="https://example.com/brelok_bmw.jpg" alt="Brelok BMW Classic">
      <h2>Brelok BMW Classic</h2>
      <p>Minimalistyczny design, logo BMW</p>
      <p class="price">34,99 zł</p>
      <button class="btn">Dodaj do koszyka</button>
    </div>

    <div class="product">
      <img src="https://example.com/brelok_audi.jpg" alt="Brelok Audi Premium">
      <h2>Brelok Audi Premium</h2>
      <p>Nowoczesny wygląd, metal + skóra</p>
      <p class="price">39,99 zł</p>
      <button class="btn">Dodaj do koszyka</button>
    </div>

    <div class="product">
      <img src="https://example.com/brelok_mercedes.jpg" alt="Brelok Mercedes Sport">
      <h2>Brelok Mercedes Sport</h2>
      <p>Sportowy styl z logiem Mercedes-Benz</p>
      <p class="price">37,99 zł</p>
      <button class="btn">Dodaj do koszyka</button>
    </div>

    <div class="product">
      <img src="https://example.com/brelok_toyota.jpg" alt="Brelok Toyota Urban">
      <h2>Brelok Toyota Urban</h2>
      <p>Solidny brelok do codziennego użytku</p>
      <p class="price">31,99 zł</p>
      <button class="btn">Dodaj do koszyka</button>
    </div>
  </div>

  <footer>
    © 2025 Breloki Samochodowe. Wszystkie prawa zastrzeżone.
  </footer>


</body></html>
