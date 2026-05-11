<!DOCTYPE html>
<html>
<head>
  <title>Birthday Surprise 🎂</title>

  <style>
    body {
      text-align: center;
      font-family: Arial;
      background-color: #ffe6f0;
      padding-top: 80px;
    }

    h1 {
      color: #ff4081;
    }

    p {
      font-size: 20px;
    }

    button {
      padding: 10px 20px;
      font-size: 18px;
      margin-top: 20px;
      border: none;
      border-radius: 10px;
      background-color: #ff4081;
      color: white;
      cursor: pointer;
    }

    button:hover {
      background-color: #e91e63;
    }

    #message {
      display: none;
      margin-top: 40px;
    }
  </style>
</head>

<body>

  <div id="questions">
    <h1>Answer These Questions 😄</h1>

    <p>Are you an amazing person?</p>
    <button onclick="nextQuestion1()">Yes</button>

    <div id="q2" style="display:none;">
      <p>Do you deserve the best birthday ever?</p>
      <button onclick="nextQuestion2()">Absolutely</button>
    </div>

    <div id="q3" style="display:none;">
      <p>Ready for your surprise? 🎁</p>
      <button onclick="showMessage()">Yes!!!</button>
    </div>
  </div>

  <div id="message">
    <h1>Happy Birthday 🎉</h1>

    <p>Dear [Friend's Name],</p>

    <p>
      You are amazing and I’m so lucky to have you!
    </p>

    <p>
      May your day be filled with happiness, laughter,
      and lots of cake 🎂💖
    </p>

    <p><b>Have a wonderful birthday! ✨</b></p>
  </div>

  <script>
    function nextQuestion1() {
      document.getElementById("q2").style.display = "block";
    }

    function nextQuestion2() {
      document.getElementById("q3").style.display = "block";
    }

    function showMessage() {
      document.getElementById("questions").style.display = "none";
      document.getElementById("message").style.display = "block";
    }
  </script>

</body>
</html>
