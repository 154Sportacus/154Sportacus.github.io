<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Bar Menu</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #111;
      color: #f4f4f4;
      margin: 0;
      padding: 0;
      text-align: center;
    }
    header {
      padding: 1em;
      background: #222;
    }
    h1 {
      margin: 0;
    }
    nav button {
      margin: 10px;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      background: #444;
      color: #fff;
      cursor: pointer;
    }
    nav button.active {
      background: #e91e63;
    }
    section {
      display: none;
      padding: 20px;
    }
    section.active {
      display: block;
    }
    .item {
      margin: 10px 0;
    }
    .price {
      color: #e0e0e0;
    }
  </style>
</head>
<body>
  <header>
    <h1>Bar Nocturne Menu</h1>
    <nav>
      <button onclick="showSection('cocktails')" class="active">Cocktails</button>
      <button onclick="showSection('beers')">Beers</button>
      <button onclick="showSection('wines')">Wines</button>
    </nav>
  </header>
  <main>
    <section id="cocktails" class="active">
      <div class="item">Mojito <span class="price">€8</span></div>
      <div class="item">Caipirinha <span class="price">€7</span></div>
      <div class="item">Old Fashioned <span class="price">€9</span></div>
    </section>
    <section id="beers">
      <div class="item">IPA <span class="price">€5</span></div>
      <div class="item">Pilsner <span class="price">€4.5</span></div>
      <div class="item">Stout <span class="price">€6</span></div>
    </section>
    <section id="wines">
      <div class="item">Merlot <span class="price">€6</span></div>
      <div class="item">Chardonnay <span class="price">€6</span></div>
      <div class="item">Rosé <span class="price">€5.5</span></div>
    </section>
  </main>
  <script>
    function showSection(id) {
      document.querySelectorAll('section').forEach(s => s.classList.remove('active'));
      document.getElementById(id).classList.add('active');
      document.querySelectorAll('nav button').forEach(b => b.classList.remove('active'));
      document.querySelector(`nav button[onclick*="${id}"]`).classList.add('active');
    }
  </script>
</body>
</html>
