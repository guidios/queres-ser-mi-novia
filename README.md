<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>¿Quieres ser mi novia?</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <div class="container">
    <h1>¿Quieres ser mi novia?</h1>
    <div class="answers">
      <button id="yes-btn">Sí</button>
      <button id="no-btn">No</button>
    </div>
  </div>
  <script>
    const yesButton = document.getElementById('yes-btn');
    const noButton = document.getElementById('no-btn');

    yesButton.addEventListener('click', function() {
      alert('¡Gracias! Te amo');
    });

    noButton.addEventListener('click', function() {
      const fontSize = window.getComputedStyle(yesButton).getPropertyValue('font-size');
      const newSize = parseFloat(fontSize) + 2;
      yesButton.style.fontSize = newSize + 'px';
    });
  </script>
</body>
</html>
