# test1
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>إدخال الكود والمعرف</title>
  <style>
    * {
      box-sizing: border-box;
      font-family: 'Tahoma', sans-serif;
    }

    body {
      margin: 0;
      height: 100vh;
      background: url('your-image.jpg') no-repeat center center fixed;
      background-size: cover;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
    }

    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.6);
    }

    .container {
      position: relative;
      z-index: 1;
      background: rgba(0, 0, 0, 0.7);
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 0 20px #ff0000;
      width: 300px;
      text-align: center;
    }

    input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: none;
      border-radius: 5px;
      text-align: center;
    }

    button {
      width: 100%;
      padding: 10px;
      background: #ff0000;
      border: none;
      border-radius: 5px;
      color: white;
      font-weight: bold;
      cursor: pointer;
      transition: 0.3s;
    }

    button:hover {
      background: #cc0000;
    }
  </style>
</head>
<body>
  <div class="overlay"></div>
  <div class="container">
    <h2>أدخل الكود والمعرف</h2>
    <input type="text" id="code" placeholder="أدخل الكود">
    <input type="text" id="id" placeholder="أدخل المعرف (ID)">
    <button onclick="sendData()">إرسال</button>
  </div>

  <script>
    function sendData() {
      const code = document.getElementById("code").value;
      const id = document.getElementById("id").value;

      if (!code || !id) {
        alert("الرجاء إدخال الكود والمعرف!");
        return;
      }

      alert(تم إدخال الكود: ${code}\nالمعرف: ${id});
    }
  </script>
</body>
</html>