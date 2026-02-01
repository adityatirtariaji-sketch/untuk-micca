<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Buat Kamu ❤️</title>
  <style>
    body{
      margin:0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg,#ff9a9e,#fad0c4);
      height:100vh;
      display:flex;
      justify-content:center;
      align-items:center;
      text-align:center;
      color:white;
      padding:20px;
    }
    .box{
      background: rgba(0,0,0,0.25);
      padding:25px;
      border-radius:20px;
      max-width:400px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }
    button{
      margin-top:15px;
      padding:12px 20px;
      border:none;
      border-radius:12px;
      font-size:16px;
      cursor:pointer;
    }
    .btn1{background:white;color:#ff4d6d;}
    .btn2{background:#ff4d6d;color:white;}
  </style>
</head>
<body>
  <div class="box">
    <h1>Hai Sayang 🥺❤️</h1>
    <p id="msg">Aku minta maaf ya kalau aku bikin kamu ngambek...</p>
    <button class="btn1" onclick="nextMsg()">Klik ini ya 😳</button>
    <button class="btn2" onclick="alert('YEAYY MAKASIH SAYANG 😭❤️')">Maafin aku 💕</button>
  </div>

  <script>
    const messages = [
      "Aku minta maaf ya kalau aku bikin kamu ngambek...",
      "Aku beneran sayang sama kamu 😔❤️",
      "Aku gak mau kita berantem lama-lama 🥺",
      "Ayo peluk dulu (walau virtual) 🤗",
      "Kamu jangan ngambek lama-lama yaaa 😭💕"
    ];
    let i = 0;
    function nextMsg(){
      i = (i + 1) % messages.length;
      document.getElementById("msg").innerText = messages[i];
    }
  </script>
</body>
</html>
