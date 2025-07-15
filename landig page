<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Nomad Mind | منصة الرحالة المبدعين</title>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Cairo', sans-serif;
      background: #f4f6f8;
      color: #222;
    }

    header {
      background: linear-gradient(135deg, #0066cc, #00ccaa);
      color: white;
      padding: 2rem;
      text-align: center;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }

    p {
      font-size: 1.2rem;
    }

    .countdown {
      font-size: 2rem;
      margin: 2rem 0;
      color: #444;
      text-align: center;
    }

    .form-container {
      background: white;
      margin: 2rem auto;
      padding: 2rem;
      max-width: 600px;
      border-radius: 12px;
      box-shadow: 0 5px 20px rgba(0,0,0,0.1);
    }

    label {
      display: block;
      margin-top: 1rem;
      font-weight: bold;
    }

    input, textarea {
      width: 100%;
      padding: 0.8rem;
      margin-top: 0.3rem;
      border: 1px solid #ccc;
      border-radius: 8px;
      font-family: 'Cairo', sans-serif;
    }

    button {
      margin-top: 1.5rem;
      background: #0066cc;
      color: white;
      padding: 1rem;
      border: none;
      border-radius: 8px;
      font-size: 1.1rem;
      cursor: pointer;
    }

    footer {
      text-align: center;
      font-size: 0.9rem;
      padding: 2rem;
      color: #777;
    }
  </style>
</head>
<body>

<header>
  <h1>Nomad Mind</h1>
  <p>منصة عربية للمبدعين والرحالة الرقميين - أنشئ، سافر، وازدهر!</p>
</header>

<div class="countdown">
  سيتم الإطلاق خلال: <span id="timer"></span>
</div>

<div class="form-container">
  <h2>شاركنا رأيك وكن من الأوائل</h2>
  <form>
    <label for="email">بريدك الإلكتروني:</label>
    <input type="email" id="email" placeholder="example@email.com" required>

    <label for="problem">ما هي أكبر مشكلة تواجهك كمصمم مستقل أو رحالة رقمي؟</label>
    <textarea id="problem" rows="3" placeholder="اكتب بإيجاز مشكلتك..."></textarea>

    <label for="feature">ما هي الميزة التي تتمنى وجودها في منصة تخدمك؟</label>
    <textarea id="feature" rows="3" placeholder="أخبرنا فكرتك أو توقعاتك..."></textarea>

    <button type="submit">انضم الآن</button>
  </form>
</div>

<footer>
  © 2025 Nomad Mind. جميع الحقوق محفوظة.
</footer>

<script>
  // إعداد العداد التنازلي
  const launchDate = new Date("August 1, 2025 00:00:00").getTime();
  const timer = document.getElementById("timer");

  setInterval(() => {
    const now = new Date().getTime();
    const distance = launchDate - now;

    const days = Math.floor(distance / (1000 * 60 * 60 * 24));
    const hrs = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const mins = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    const secs = Math.floor((distance % (1000 * 60)) / 1000);

    if (distance < 0) {
      timer.innerHTML = "تم الإطلاق!";
    } else {
      timer.innerHTML = `${days} يوم - ${hrs} ساعة - ${mins} دقيقة - ${secs} ثانية`;
    }
  }, 1000);
</script>

</body>
</html>
