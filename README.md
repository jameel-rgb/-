<!doctype html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>اتصل بنا - متجر جميل</title>
  <style>
    :root{--accent:#0b74de;--bg:#f7f7f9}
    body{font-family: Tahoma, 'Segoe UI', Roboto, Arial; background:var(--bg); margin:0; color:#222}
    header{background:white;padding:18px 20px;display:flex;align-items:center;justify-content:space-between;box-shadow:0 1px 6px rgba(0,0,0,0.06)}
    .brand{display:flex;align-items:center;gap:12px}
    .brand .logo{width:44px;height:44px;border-radius:8px;background:linear-gradient(135deg,var(--accent),#4fb1ff);display:flex;align-items:center;justify-content:center;color:white;font-weight:700}
    nav a{margin-left:12px;color:#555;text-decoration:none;font-weight:500}
    nav a:hover{color:var(--accent)}
    main{max-width:800px;margin:26px auto;padding:0 16px}
    h1{margin-bottom:12px}
    .contact-form{background:white;padding:22px;border-radius:12px;box-shadow:0 1px 6px rgba(0,0,0,0.06);display:flex;flex-direction:column;gap:12px}
    .contact-form input, .contact-form textarea{padding:10px;border-radius:6px;border:1px solid #ddd;width:100%}
    .contact-form button{padding:10px;border-radius:8px;border:none;background:var(--accent);color:white;font-weight:600}
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <div class="logo">ج</div>
      <div>
        <div style="font-weight:700">متجر جميل</div>
        <div style="font-size:13px;color:#666">بيع كل شيء جميل ومطلوب — داخل فلسطين فقط</div>
      </div>
    </div>
    <nav>
      <a href="index.html">الرئيسية</a>
      <a href="contact.html">اتصل بنا</a>
    </nav>
  </header>

  <main>
    <h1>اتصل بنا</h1>
    <p>يمكنك التواصل معنا عبر النموذج أدناه، وسنقوم بالرد في أقرب وقت.</p>
    <form class="contact-form" id="contactForm">
      <input type="text" name="name" placeholder="الاسم الكامل" required>
      <input type="email" name="email" placeholder="البريد الإلكتروني" required>
      <input type="tel" name="phone" placeholder="رقم الهاتف" required>
      <textarea name="message" rows="5" placeholder="رسالتك" required></textarea>
      <button type="submit">إرسال الرسالة</button>
    </form>
  </main>

  <footer style="text-align:center;padding:20px;color:#666;font-size:14px">
    © جميع الحقوق محفوظة — متجر جميل. جاهز للبيع داخل فلسطين.
  </footer>

  <script>
    document.getElementById('contactForm').addEventListener('submit', function(e){
      e.preventDefault();
      alert('تم استلام رسالتك! سنتواصل معك قريبًا.');
      this.reset();
    });
  </script>
</body>
</html>
