# Sorry-bhumu<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>I’m Sorry 💔</title>
  <style>
    body {
      background-color: #000;
      margin: 0;
      overflow: hidden;
      font-family: sans-serif;
    }

    .sorry {
      position: absolute;
      font-size: 24px;
      font-weight: bold;
      animation: fadeOut 3s ease-out forwards;
    }

    @keyframes fadeOut {
      0% {opacity: 1;}
      100% {opacity: 0; transform: scale(1.5);}
    }

    h1 {
      color: white;
      text-align: center;
      margin-top: 30vh;
      font-size: 2.5rem;
    }
  </style>
</head>
<body>
  <h1>Touch Anywhere 🥺</h1>
  <script>
    const colors = ['red', 'yellow', 'pink', 'lightblue', 'orange', 'violet', 'lime', 'magenta'];

    document.body.addEventListener("click", showSorry);
    document.body.addEventListener("touchstart", showSorry);

    function showSorry(e) {
      const text = document.createElement("div");
      text.classList.add("sorry");
      text.innerText = "Sorryyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyyy Bhumuuuuuuuuuuuu 🥺🥺🥺😭😭😭🙏🙏 Maaf kardooooo";
      text.style.color = colors[Math.floor(Math.random() * colors.length)];

      text.style.left = `${Math.random() * window.innerWidth}px`;
      text.style.top = `${Math.random() * window.innerHeight}px`;

      document.body.appendChild(text);

      setTimeout(() => {
        text.remove();
      }, 3000);
    }
  </script>
</body>
</html>
