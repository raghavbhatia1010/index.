<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Valentine 💗</title>

  <style>
    body {
      margin: 0;
      height: 100vh;
      background: #f6e8dc; /* beige */
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Georgia', serif;
    }

    .card {
      background: #f9c5d1; /* soft pink */
      padding: 40px 30px;
      border-radius: 18px;
      text-align: center;
      max-width: 420px;
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
    }

    .message {
      font-size: 15px;
      color: #5a2a3a;
      margin-bottom: 20px;
      line-height: 1.6;
    }

    h1 {
      font-size: 24px;
      color: #4a1f2d;
      margin-bottom: 25px;
    }

    .buttons {
      display: flex;
      justify-content: center;
      gap: 20px;
    }

    button {
      padding: 12px 24px;
      font-size: 16px;
      border: none;
      border-radius: 25px;
      cursor: pointer;
      transition: all 0.3s ease;
    }

    .yes {
      background: #fff;
      color: #c94a6a;
      font-weight: bold;
    }

    .yes:hover {
      background: #ffe6ee;
    }

    .no {
      background: #f1a7b8;
      color: #fff;
      position: relative;
    }
  </style>
</head>

<body>
  <div class="card">
    <div class="message">
      <strong>Hey Kyra,</strong><br>
      I’m sorry I couldn’t do this earlier — there’s been a lot going on lately.
      This might not be much, but I’m making use of whatever I have at my disposal.
      <br><br>
      <strong>P.S.</strong> I’m really looking forward to seeing you in the UK. x
    </div>

    <h1>Kyra, will you be my Valentine?</h1>

    <div class="buttons">
      <button class="yes" onclick="yesClicked()">Yes</button>
      <button class="no" onmouseover="moveNo(this)">No</button>
    </div>
  </div>

  <script>
    function yesClicked() {
      document.body.innerHTML = `
        <div style="
          height:100vh;
          display:flex;
          justify-content:center;
          align-items:center;
          background:#f6e8dc;
          font-family:Georgia, serif;
          text-align:center;">
          <h1 style="color:#c94a6a;">
            You just made me really happy 💗
          </h1>
        </div>
      `;
    }

    function moveNo(btn) {
      btn.style.top = Math.random() * 60 - 30 + "px";
      btn.style.left = Math.random() * 60 - 30 + "px";
    }
  </script>
</body>
</html>
