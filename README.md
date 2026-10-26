
<!DOCTYPE html>
<html lang="hi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pk Boss Market</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f3f6fb;
      color: #172033;
    }
    header {
      background: #123b72;
      color: white;
      padding: 22px 16px;
      text-align: center;
    }
    .container {
      max-width: 600px;
      margin: 25px auto;
      padding: 16px;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 14px;
      margin-bottom: 16px;
      box-shadow: 0 3px 12px #00000010;
    }
    button {
      background: #145bd7;
      color: white;
      border: 0;
      padding: 12px 18px;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }
    input {
      box-sizing: border-box;
      width: 100%;
      padding: 12px;
      margin: 8px 0 14px;
      border: 1px solid #ccd3df;
      border-radius: 8px;
      font-size: 16px;
    }
    #message { color: #145bd7; }
  </style>
</head>
<body>
  <header>
    <h1>PK BOSS MARKET</h1>
    <p>Welcome to Our Market</p>
  </header>

  <main class="container">
    <section class="card">
      <h2>हमारी मार्केट में आपका स्वागत है!</h2>
      <p>यह आपकी Pk Boss Market ऐप की शुरुआत है।</p>
      <button onclick="showMessage()">शुरू करें</button>
      <p id="message"></p>
    </section>

    <section class="card">
      <h2>संपर्क करें</h2>
      <form onsubmit="sendMessage(event)">
        <label for="name">आपका नाम</label>
        <input id="name" required placeholder="नाम लिखें">

        <label for="phone">मोबाइल नंबर</label>
        <input id="phone" type="tel" required placeholder="मोबाइल नंबर लिखें">

        <button type="submit">जानकारी भेजें</button>
      </form>
      <p id="formMessage"></p>
    </section>
  </main>

  <script>
    function showMessage() {
      document.getElementById("message").textContent =
        "धन्यवाद! Pk Boss Market में आपका स्वागत है।";
    }

    function sendMessage(event) {
      event.preventDefault();
      document.getElementById("formMessage").textContent =
        "डेमो फॉर्म है। आपकी जानकारी अभी किसी सर्वर पर नहीं भेजी गई है।";
    }
  </script>
</body>
</html>
