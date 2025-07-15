
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
      padding: 2rem 1rem;
      text-align: center;
    }

    h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }

    p {
      font-size: 1.2rem;
      margin: 0;
    }

    .countdown {
      font-size: 2rem;
      margin: 2rem 0;
      color: #444;
      text-align: center;
    }

    /* ====== Sections (Problems + Features) ====== */
    .section {
      background: #ffffff;
      margin: 2rem auto;
      padding: 2rem 1.5rem;
      max-width: 800px;
      border-radius: 12px;
      box-shadow: 0 5px 20px rgba(0,0,0,0.05);
    }

    .section h2 {
      font-size: 1.8rem;
      margin-bottom: 1rem;
      color: #0066cc;
    }

    .section ul {
      list-style: none;
      padding: 0;
    }

    .section li {
      margin: 0.7rem 0;
      line-height: 1.6;
      display: flex;
      align-items: flex-start;
    }

    .section li::before {
      content: "✓";
      margin-left: 0.5rem;
      color: #00ccaa;
      font-weight: bold;
    }

    /* ====== Form ====== */
    .form-container {
      background: #ffffff;
      margin: 2rem auto;
      padding: 2rem 1.5rem;
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
      transition: background 0.3s ease;
    }

    button:hover {
      background: #0055aa;
    }

    footer {
      text-align: center;
      font-size: 0.9rem;
      padding: 2rem 1rem;
      color: #777;
    }
  </style>
</head>
<body>

<header>
  <h1>Nomad Mind</h1>
  <p>منصة عربية للمبدعين والرحالة الرقميين - أنشئ، سافر، وازدهر!</p>
</header>

<!-- ====== Countdown ====== -->
<div class="countdown">
  سيتم الإطلاق خلال: <span id="timer"></span>
</div>

<!-- ====== Problems Section ====== -->
<section class="section" id="problems">
  <h2>المشكلات التي نحلها</h2>
  <ul>
    <li>صعوبة العثور على منصة عربية متكاملة لبيع التصاميم الرقمية.</li>
    <li>محدودية الوصول لعملاء جدد دون تكاليف تسويقية مرتفعة.</li>
    <li>غياب أدوات تُسهِّل نمط حياة الرحالة الرقميين وتربطهم بفرص عمل.</li>
    <li>الحاجة لإرشاد ذكي لاتخاذ قرارات حول السفر، العمل، والتوازن بينهما.</li>
  </ul>
</section>

<!-- ====== Features Section ====== -->
<section class="section" id="features">
  <h2>مميزات Nomad Mind</h2>
  <ul>
    <li>متجر شخصي مجاني وسهل لبيع التصاميم والمنتجات الرقمية.</li>
    <li>تسويق تلقائي يعتمد على الذكاء الاصطناعي للوصول إلى العملاء المستهدفين.</li>
    <li>مجتمع تفاعلي يجمع المصممين، الفريلانسرز، والرحالة الرقميين.</li>
    <li>مساعد ذكي يقدم توصيات حول فرص العمل وأماكن الإقامة والعمل المشترك.</li>
    <li>لوحة تحكم مبسطة لمتابعة المبيعات، التحليلات، وإدارة المنتجات.</li>
  </ul>
</section>

<!-- ====== Form Section ====== -->
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
