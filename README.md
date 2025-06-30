<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Badak Store - Topup Game Murah</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background: #f0f9ff;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #00c851;
      color: white;
      text-align: center;
      padding: 1rem;
    }
    main {
      padding: 2rem;
    }
    h1 {
      color: #007e33;
    }
    .game-list, form {
      max-width: 600px;
      margin: auto;
    }
    .game-item {
      padding: 10px;
      border: 1px solid #ccc;
      background: white;
      margin: 5px 0;
      border-radius: 5px;
    }
    form input, form select, form button {
      display: block;
      width: 100%;
      margin-top: 10px;
      padding: 10px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    form button {
      background-color: #ffbb33;
      color: white;
      font-weight: bold;
      border: none;
      cursor: pointer;
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #007e33;
      color: white;
    }
  </style>
</head>
<body>
  <header>
    <h1>Badak Store</h1>
    <p>Topup murah, cepat, aman, dan terjamin 100%</p>
  </header>

  <main>
    <h2>Pilih Game</h2>
    <div class="game-list">
      <div class="game-item">Mobile Legends</div>
      <div class="game-item">Free Fire</div>
      <div class="game-item">PUBG Mobile</div>
      <div class="game-item">Genshin Impact</div>
      <div class="game-item">Valorant</div>
      <div class="game-item">Call of Duty Mobile</div>
    </div>

    <h2>Form Pemesanan</h2>
    <form id="orderForm">
      <input type="text" id="game" placeholder="Nama Game (misal: Mobile Legends)" required />
      <input type="text" id="id" placeholder="User ID / Server" required />
      <input type="text" id="nominal" placeholder="Nominal (misal: 86 Diamond)" required />
      <input type="text" id="nama" placeholder="Nama Kamu" required />
      <button type="submit">Order Sekarang</button>
    </form>
  </main>

  <footer>
    <p>&copy; 2025 Badak Store. Semua Hak Dilindungi.</p>
  </footer>

  <script>
    const form = document.getElementById('orderForm');
    form.addEventListener('submit', function (e) {
      e.preventDefault();
      const game = document.getElementById('game').value;
      const id = document.getElementById('id').value;
      const nominal = document.getElementById('nominal').value;
      const nama = document.getElementById('nama').value;

      const message = `Halo Admin Badak Store!%0ASaya ingin top-up game:%0A- Game: ${game}%0A- ID/Server: ${id}%0A- Nominal: ${nominal}%0A- Nama: ${nama}`;
      const phone = '62895395214769';
      const url = `https://wa.me/${phone}?text=${message}`;
      window.open(url, '_blank');
    });
  </script>
</body>
</html>
