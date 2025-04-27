<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>دفع - LEADER STORE</title>

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

<header>
  صفحة الدفع - LEADER STORE
</header>

<div class="payment-form">
  <h2> بيانات الدفع</h2>
  
  <form action="/submit_payment" method="POST">
    <!-- الاسم  -->
    <label for="customerName">الاسم :</label>
    <input type="text" id="customerName" name="customerName" class="readonly" value="leader المئذي  " readonly>

    <!-- رقم الهاتف -->
    <label for="phoneNumber">رقم الهاتف:</label>
    <input type="tel" id="phoneNumber" name="phoneNumber" class="readonly" value="+905318189272" readonly>

    <!-- المبلغ -->
    <label for="amount">المبلغ:</label>
    <input type="number" id="amount" name="amount" class="readonly" value="100" readonly>

    <!-- IBAN -->
    <label for="iban">رقم IBAN (رقم الحساب المصرفي):</label>
    <input type="text" id="iban" name="iban" class="readonly" value="TR330006100519786257310001" readonly>
    
    <!-- زر الدفع -->
    <button type="submit">إتمام الدفع</button>
  </form>
</div>

<footer>
  &copy; جميع الحقوق محفوظة LEADER 2050 | للتواصل: Discord: A7_AB | هاتف: +905318189272
</footer>

</body>
</html>
