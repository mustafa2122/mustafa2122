<!DOCTYPE html>
<html>
<head>
  <title>حجز المصور مصطفى عبد الحميد</title>
  <style>
    /* أنماط CSS لتنسيق الصفحة */
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f1f1f1;
    }

    .container {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
    }

    h1 {
      text-align: center;
    }

    form {
      background-color: #fff;
      padding: 20px;
      border-radius: 5px;
    }

    label {
      display: block;
      margin-bottom: 10px;
    }

    input[type="text"],
    input[type="email"],
    input[type="date"],
    textarea {
      width: 100%;
      padding: 8px;
      border: 1px solid #ccc;
      border-radius: 4px;
      box-sizing: border-box;
    }

    input[type="submit"] {
      background-color: #4CAF50;
      color: #fff;
      padding: 10px 15px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
      float: right;
    }

    input[type="submit"]:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>حجز المصور مصطفى عبد الحميد</h1>
    <form>
      <label for="name">الاسم:</label>
      <input type="text" id="name" name="name" required>

      <label for="email">البريد الإلكتروني:</label>
      <input type="email" id="email" name="email" required>

      <label for="date">تاريخ الحجز:</label>
      <input type="date" id="date" name="date" required>

      <label for="message">ملاحظات إضافية:</label>
      <textarea id="message" name="message" rows="4"></textarea>

      <input type="submit" value="حجز">
    </form>
  </div>

  <script>
    // تنفيذ إجراء الحجز عند النقر على زر الحجز
    document.querySelector('form').addEventListener('submit', function(event) {
      event.preventDefault(); // منع إعادة تحميل الصفحة

      // استخراج قيم الحقول
      var name = document.getElementById('name').value;
      var email = document.getElementById('email').value;
      var date = document.getElementById('date').value;
      var message = document.getElementById('message').value;

      // هنا يمكنك إجراء الإجراءات اللازمة مثل إرسال البيانات إلى خادم أو تنفيذ العمليات اللازمة

      // مثال بسيط: عرض رسالة تأكيد بعد حجز ناجح
      alert('تم حجز المصور بنجاح!');

      // مسح قيم الحقول
      document.getElementById('name').value = '';
      document.getElementById('email').value = '';
      document.getElementById('date').value = '';
      document.getElementById('message').value = '';
    });
  </script>
</body>
</html>
