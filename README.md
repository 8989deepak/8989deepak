<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Proposal Target Shoot Game</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
    }
    #container {
      margin-top: 100px;
    }
    #target {
      width: 100px;
      height: 100px;
      background-color: red;
      position: relative;
    }
  </style>
</head>
<body>
  <div id="container">
    <h1>Do you love me?</h1>
    <div id="target"></div>
  </div>

  <script>
    const target = document.getElementById('target');
    const container = document.getElementById('container');

    target.addEventListener('click', () => {
      target.style.marginLeft = `${Math.random() * 80}vw`;
      target.style.marginTop = `${Math.random() * 80}vh`;
      container.innerHTML = '<h1>Yes!</h1><p>Thank you! I love you too!</p>';
    });
  </script>
</body>
</html>
