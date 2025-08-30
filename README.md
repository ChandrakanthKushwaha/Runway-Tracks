 <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Runway Tracks</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f4f4;
      color: #333;
    }
    header {
      background: linear-gradient(90deg, #000, #444);
      color: #fff;
      padding: 20px;
      text-align: center;
      font-size: 28px;
      font-weight: bold;
      letter-spacing: 2px;
    }
    nav {
      text-align: center;
      background: #111;
      padding: 10px 0;
    }
    nav a {
      margin: 0 15px;
      text-decoration: none;
      color: #fff;
      font-weight: 500;
    }
    nav a:hover { color: #e0b100; }
    .hero {
      background: url('https://via.placeholder.com/1400x500/000000/ffffff?text=Runway+Tracks') no-repeat center center/cover;
      color: #fff;
      padding: 100px 20px;
      text-align: center;
    }
    .hero h1 {
      font-size: 50px;
      margin-bottom: 15px;
      text-shadow: 2px 2px 8px rgba(0,0,0,0.6);
    }
    .hero p { font-size: 22px; margin-bottom: 30px; }
    .button {
      background-color: #e0b100;
      color: #000;
      padding: 14px 30px;
      text-decoration: none;
      border-radius: 25px;
      font-weight: bold;
      display: inline-block;
      margin: 8px;
      transition: 0.3s;
    }
    .button:hover { background-color: #ffcc00; }
    .products {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      padding: 50px 20px;
      background: #fff;
    }
    .product {
      background: #fafafa;
      border-radius: 15px;
      box-shadow: 0 6px 12px rgba(0,0,0,0.1);
      margin: 20px;
      padding: 25px;
      width: 300px;
      text-align: center;
      transition: transform 0.3s;
    }
    .product:hover { transform: scale(1.05); }
    .product img {
      width: 100%;
      border-radius: 15px;
      margin-bottom: 20px;
    }
    .product h3 { margin-bottom: 10px; font-size: 22px; }
    .product p {
      font-size: 18px;
      margin-bottom: 15px;
      color: #e63946;
      font-weight: bold;
    }
    .referral {
      background: linear-gradient(90deg, #111, #444);
      color: #fff;
      padding: 40px 20px;
      text-align: center;
      font-size: 22px;
      font-weight: bold;
    }
    footer {
      background: #000;
      color: #fff;
      text-align: center;
      padding: 20px;
      font-size: 15px;
    }
    footer a { color: #e0b100; text-decoration: none; }
    /* Referral Popup */
    .popup {
      display: none;
      position: fixed;
      z-index: 1000;
      left: 0; top: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.6);
    }
    .popup-content {
      background: #fff;
      border-radius: 15px;
      padding: 25px;
      width: 80%;
      max-width: 600px;
      margin: 80px auto;
      text-align: center;
      position: relative;
    }
    .popup-content h2 { margin-top: 0; }
    .popup-content input {
      width: 90%; padding: 12px; margin: 10px 0;
      border: 1px solid #ccc; border-radius: 8px;
    }
    .popup-content button {
      background: #e0b100;
      border: none;
      padding: 12px 25px;
      border-radius: 20px;
      cursor: pointer;
      font-weight: bold;
    }
    .popup-content button:hover { background: #ffcc00; }
    .popup-content span {
      position: absolute;
      right: 15px; top: 10px;
      font-size: 24px; cursor: pointer; color: #444;
    }
    /* Referrals table */
    #referralsTable {
      width: 100%;
      border-collapse: collapse;
      margin-top: 15px;
      font-size: 15px;
    }
    #referralsTable th, #referralsTable td {
      padding: 10px; border: 1px solid #ddd;
      text-align: center;
    }
    #referralsTable th {
      background: #000; color: #fff;
    }
    /* Mobile */
    @media(max-width: 768px) {
      .hero h1 { font-size: 36px; }
      .hero p { font-size: 18px; }
      .products { flex-direction: column; align-items: center; }
      .product { width: 90%; }
    }
  </style>
</head>
<body>
  <header>Runway Tracks</header>

  <nav>
    <a href="#home">Home</a>
    <a href="#shop">Shop</a>
    <a href="#referral">Referral Offer</a>
    <a href="#contact">Contact</a>
  </nav>

  <section class="hero" id="home">
    <h1>Runway Tracks</h1>
    <p>Style in Motion – Refer & Earn ₹100 on Every Referral!</p>
    <a href="tel:9502907095" class="button">📞 Call Now</a>
    <a href="https://wa.me/919502907095?text=Hi%20I%20want%20to%20order%20Track%20Pants" target="_blank" class="button">💬 WhatsApp Order</a>
  </section>

  <section class="products" id="shop">
    <div class="product">
      <img src="https://via.placeholder.com/300x350/111111/ffffff?text=Track+Pants" alt="Track Pants">
      <h3>Classic Track Pants</h3>
      <p>₹599 per pair</p>
      <a href="tel:9502907095" class="button">📞 Call to Order</a>
      <a href="https://wa.me/919502907095?text=Hi%20I%20want%20to%20order%20Track%20Pants" target="_blank" class="button">💬 WhatsApp Order</a>
    </div>
  </section>

  <section class="referral" id="referral">
    🎉 Refer & Earn ₹100 on Every Referral! <br>
    <button id="openForm" class="button">➕ Submit Referral</button>
    <button id="viewReferrals" class="button">📋 View My Referrals</button>
  </section>

  <!-- Referral Form Popup -->
  <div id="referralPopup" class="popup">
    <div class="popup-content">
      <span id="closePopup">&times;</span>
      <h2>Submit Referral</h2>
      <input type="text" id="refName" placeholder="Your Name">
      <input type="text" id="friendName" placeholder="Friend's Name">
      <input type="text" id="friendPhone" placeholder="Friend's Phone">
      <button id="submitReferral">Submit</button>
    </div>
  </div>

  <!-- Referrals List Popup -->
  <div id="referralsPopup" class="popup">
    <div class="popup-content">
      <span id="closeReferrals">&times;</span>
      <h2>📋 My Referrals</h2>
      <table id="referralsTable">
        <thead>
          <tr><th>Name</th><th>Friend</th><th>Phone</th><th>Date</th></tr>
        </thead>
        <tbody><tr><td colspan="4">Loading...</td></tr></tbody>
      </table>
      <h3 id="totalBonus" style="margin-top:15px; color:#e0b100; text-align:right;">
        Total Bonus: ₹0
      </h3>
    </div>
  </div>

  <footer id="contact">
    📞 Contact: <a href="tel:9502907095">9502907095</a> <br>
    💬 WhatsApp: <a href="https://wa.me/919502907095" target="_blank">Chat Now</a> <br>
    © 2025 Runway Tracks. All rights reserved.
  </footer>

  <script>
    const referralPopup = document.getElementById("referralPopup");
    const openForm = document.getElementById("openForm");
    const closePopup = document.getElementById("closePopup");
    const submitReferral = document.getElementById("submitReferral");

    const referralsPopup = document.getElementById("referralsPopup");
    const viewReferrals = document.getElementById("viewReferrals");
    const closeReferrals = document.getElementById("closeReferrals");
    const referralsTable = document.getElementById("referralsTable").getElementsByTagName("tbody")[0];
    const totalBonus = document.getElementById("totalBonus");

    // Open/close referral form
    openForm.onclick = () => referralPopup.style.display = "block";
    closePopup.onclick = () => referralPopup.style.display = "none";

    // Submit referral to Google Sheets
    submitReferral.onclick = () => {
      const name = document.getElementById("refName").value;
      const friend = document.getElementById("friendName").value;
      const phone = document.getElementById("friendPhone").value;

      if (!name || !friend || !phone) {
        alert("Please fill all fields.");
        return;
      }

      fetch("YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL", {
        method: "POST",
        body: JSON.stringify({ name, friend, phone }),
        headers: { "Content-Type": "application/json" }
      })
      .then(res => res.text())
      .then(() => {
        alert("Referral submitted!");
        referralPopup.style.display = "none";
      })
      .catch(() => alert("Error submitting referral."));
    };

    // View referrals
    viewReferrals.onclick = () => {
      referralsPopup.style.display = "block";
      referralsTable.innerHTML = "<tr><td colspan='4'>⏳ Loading...</td></tr>";
      totalBonus.textContent = "Total Bonus: ₹0";

      fetch("YOUR_GOOGLE_SHEET_JSON_URL")
        .then(res => res.json())
        .then(data => {
          referralsTable.innerHTML = "";
          let count = 0;
          data.forEach(row => {
            const tr = document.createElement("tr");
            tr.innerHTML = `<td>${row.name}</td><td>${row.friend}</td><td>${row.phone}</td><td>${row.date}</td>`;
            referralsTable.appendChild(tr);
            count++;
          });
          totalBonus.textContent = `💰 Total Bonus: ₹${count * 100}`;
        })
        .catch(() => {
          referralsTable.innerHTML = "<tr><td colspan='4'>❌ Failed to load referrals</td></tr>";
        });
    };

    closeReferrals.onclick = () => referralsPopup.style.display = "none";
    window.onclick = (e) => {
      if (e.target === referralPopup) referralPopup.style.display = "none";
      if (e.target === referralsPopup) referralsPopup.style.display = "none";
    };
  </script>
</body>
</html>
