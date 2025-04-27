<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>دفع - 𝐓𝐡𝐞 𝐋𝐚𝐬𝐭 𝐒𝐓𝐎𝐑𝐄</title>

  <style>
    body {
      font-family: 'Cairo', sans-serif;
      background: linear-gradient(to right, #000000, #111111);
      color: #ffd700;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #111;
      color: #ffd700;
      padding: 20px;
      text-align: center;
      font-size: 2em;
      box-shadow: 0 8px 20px rgba(255, 215, 0, 0.5);
    }

    .payment-form {
      max-width: 600px;
      margin: 50px auto;
      padding: 20px;
      background: #222;
      border-radius: 10px;
      box-shadow: 0 10px 20px rgba(255, 215, 0, 0.4);
    }

    .payment-form label {
      display: block;
      margin-bottom: 10px;
      font-size: 1.1em;
      color: #ffd700;
    }

    .payment-form input, .payment-form button {
      width: 100%;
      padding: 10px;
      margin-bottom: 20px;
      border: none;
      border-radius: 5px;
      font-size: 1em;
    }

    .payment-form input {
      background-color: #333;
      color: #ffd700;
    }

    .payment-form button {
      background-color: #ffd700;
      color: #111;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.3s ease;
    }

    .payment-form button:hover {
      background-color: #e6c200;
    }

    footer {
      background-color: #111;
      text-align: center;
      color: #ffd700;
      padding: 20px;
      font-size: 1em;
    }

    /* تأثير الحقول القابلة للنسخ */
    .readonly {
      background-color: #444;
      color: #ffd700;
      cursor: text;
    }

    .readonly::selection {
      background: #ffd700;
      color: #111;
    }
  </style>
</head>
<body>

    <!-- أزرار التواصل الثابتة مع نوافذ منبثقة (Tooltips) -->
    <div class="social-buttons">
      <a href="https://discord.gg/QaZpgeSrQJ" target="_blank" class="social-btn" id="discord-btn">
        <img src="https://i.imgur.com/dju0Uyt.png" a>
     
      </a>
    </div>
<header>
  صفحة الدفع - 𝐓𝐡𝐞 𝐋𝐚𝐬𝐭 𝐒𝐓𝐎𝐑𝐄
</header>

<div class="payment-form">
  <h2> بيانات الدفع</h2>
  
  <form action="/submit_payment" method="POST">
    <!-- الاسم  -->
    <label for="customerName">الاسم :</label>
    <input type="text" id="customerName" name="customerName" class="readonly" value="𝐓𝐡𝐞 𝐋𝐚𝐬𝐭 𝐒𝐓𝐎𝐑𝐄  " readonly>

    <!-- ديسكورد -->
    <label for="phoneNumber">ديسكورد :</label>
    <input type="tel" id="phoneNumber" name="phoneNumber" class="readonly" value="A7_AB" readonly>

    <!-- المبلغ -->
    <label for="amount">المبلغ:</label>
    <input type="number" id="amount" name="amount" class="readonly" value="وفقا لمشترياتك تقوم بلارسال" readonly>

    <!-- IBAN -->
    <label for="iban"> PayPal (ايميل الحساب المصرفي) </label>
    <input type="text" id="PayPal" name="PayPal" class="readonly" value="ahmedalail746@gmail.com" readonly>
    
    <!-- زر الدفع -->
    <button type="button" onclick="alert('يرجى نسخ بيانات الدفع والتحويل يدوياً')">إتمام الدفع</button>

  </form>
</div>

<footer>
  &copy; جميع الحقوق محفوظة 𝐓𝐡𝐞 𝐋𝐚𝐬𝐭 𝐒𝐓𝐎𝐑𝐄 2025 | للتواصل: Discord: A7_AB |
</footer>

</body>
</html>
