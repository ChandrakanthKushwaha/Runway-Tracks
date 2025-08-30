<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Runway Tracks</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #000, #111, #000);
      color: #fff;
    }
    header {
      text-align: center;
      padding: 40px 20px;
    }
    header h1 {
      font-size: 50px;
      color: gold;
      margin-bottom: 10px;
    }
    header p {
      margin: 5px 0;
      font-size: 18px;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 40px;
    }
    .product {
      background: #1a1a1a;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 6px 12px rgba(0,0,0,0.4);
      text-align: center;
      transition: transform 0.3s;
    }
    .product:hover {
      transform: scale(1.05);
    }
    .product img {
      width: 100%;
      height: 350px;
      object-fit: cover;
    }
    .product h3 {
      margin: 15px 0 5px;
      font-size: 22px;
    }
    .product p {
      font-size: 18px;
      color: gold;
      font-weight: bold;
    }
    .button {
      display: inline-block;
      background: gold;
      color: black;
      padding: 10px 20px;
      border-radius: 25px;
      margin: 10px 5px;
      font-weight: bold;
      text-decoration: none;
      transition: 0.3s;
    }
    .button:hover {
      background: #ffcc00;
    }
    .referral {
      background: #111;
      text-align: center;
      padding: 40px 20px;
      font-size: 22px;
      font-weight: bold;
      color: gold;
    }
    .referral-form {
      max-width: 500px;
      margin: 20px auto;
      background: #1a1a1a;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 6px 12px rgba(0,0,0,0.4);
    }
    .referral-form h2 {
      text-align: center;
      margin-bottom: 20px;
      color: gold;
    }
    .referral-form label {
      display: block;
      margin: 10px 0 5px;
      font-size: 16px;
    }
    .referral-form input {
      width: 100%;
      padding: 10px;
      border-radius: 8px;
      border: none;
      margin-bottom: 15px;
      font-size: 16px;
    }
    .referral-form button {
      width: 100%;
      padding: 12px;
      border: none;
      border-radius: 25px;
      background: gold;
      color: black;
      font-weight: bold;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
    }
    .referral-form button:hover {
      background: #ffcc00;
    }
    footer {
      text-align: center;
      padding: 20px;
      background: #000;
      color: #ccc;
      font-size: 15px;
    }
    footer a {
      color: gold;
      text-decoration: none;
    }
  </style>
</head>
<body>

  <header>
    <h1>Runway Tracks</h1>
    <p>Premium Track Pants at Just ₹599</p>
    <p>Refer & Earn ₹100 on Every Referral!</p>
    <p>📞 Contact: <a href="tel:9502907095" style="color:gold;">9502907095</a></p>
  </header>

  <section class="products">
    <div class="product">
      <img src="track1.png" alt="Track Pants 1">
      <h3>Runway Tracks</h3>
      <p>₹599</p>
      <a href="tel:9502907095" class="button">📞 Call to Order</a>
      <a href="https://wa.me/919502907095?text=Hi%20I%20want%20to%20order%20Track%20Pants" target="_blank" class="button">💬 WhatsApp</a>
    </div>
    <div class="product">
      <img src="track2.png" alt="Track Pants 2">
      <h3>Runway Tracks</h3>
      <p>₹599</p>
      <a href="tel:9502907095" class="button">📞 Call to Order</a>
      <a href="https://wa.me/919502907095?text=Hi%20I%20want%20to%20order%20Track%20Pants" target="_blank" class="button">💬 WhatsApp</a>
    </div>
    <div class="product">
      <img src="track3.png" alt="Track Pants 3">
      <h3>Runway Tracks</h3>
      <p>₹599</p>
      <a href="tel:9502907095" class="button">📞 Call to Order</a>
      <a href="https://wa.me/919502907095?text=Hi%20I%20want%20to%20order%20Track%20Pants" target="_blank" class="button">💬 WhatsApp</a>
    </div>
  </section>

  <section class="referral">
    🎉 Refer Your Friends & Earn ₹100 on Every Referral!
  </section>

  <section class="referral-form">
    <h2>Referral Form</h2>
    <form action="mailto:your-email@example.com" method="post" enctype="text/plain">
      <label for="name">Your Name</label>
      <input type="text" id="name" name="name" required>

      <label for="friend">Friend's Name</label>
      <input type="text" id="friend" name="friend" required>

      <label for="phone">Friend's Phone Number</label>
      <input type="tel" id="phone" name="phone" required>

      <button type="submit">Submit Referral</button>
    </form>
  </section>

  <footer>
    📞 Call: <a href="tel:9502907095">9502907095</a> | 💬 WhatsApp: 
    <a href="https://wa.me/919502907095" target="_blank">Chat Now</a> <br>
    © 2025 Runway Tracks. All rights reserved.
  </footer>

</body>
</html>
