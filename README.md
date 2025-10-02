# HELLOBAE
BIRTHDAY LUV
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Happy Birthday, My Love!</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      background: linear-gradient(120deg, #FFEDFA, #FFB8E0, #EC7FA9, #BE5985);
      font-family: 'Segoe UI', sans-serif;
      color: #BE5985;
      margin: 0;
      padding: 0;
    }
    .container {
      max-width: 600px;
      margin: 50px auto;
      background: #FFEDFA99;
      border-radius: 16px;
      box-shadow: 0 4px 16px #EC7FA933;
      padding: 32px;
    }
    h1 {
      text-align: center;
      font-size: 2.5em;
      margin-bottom: 0.2em;
      color: #BE5985;
    }
    .love-message {
      text-align: center;
      font-size: 1.2em;
      margin-bottom: 2em;
      color: #EC7FA9;
    }
    section {
      margin-bottom: 2em;
    }
    label {
      font-weight: bold;
      color: #BE5985;
    }
    input, textarea {
      width: 100%;
      margin: 8px 0 16px 0;
      padding: 8px;
      border-radius: 8px;
      border: 1px solid #EC7FA9;
    }
    ul {
      background: #FFB8E099;
      padding: 12px;
      border-radius: 8px;
    }
    .music-list audio {
      width: 100%;
      margin-bottom: 8px;
    }
    .note {
      background: #EC7FA999;
      padding: 12px;
      border-radius: 8px;
      font-style: italic;
    }
    /* Privacy modal */
    #privacy-modal {
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background: #FFEDFAEE;
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 10;
    }
    #privacy-modal-content {
      background: #FFB8E0;
      padding: 24px;
      border-radius: 16px;
      box-shadow: 0 2px 8px #BE598599;
      text-align: center;
      min-width: 350px;
      min-height: 350px;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    #special-box {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 24px;
    }
    #special-box img {
      max-width: 90%;
      border-radius: 12px;
      margin-bottom: 10px;
      box-shadow: 0 2px 8px #BE598544;
    }
    #special-box h1 {
      font-size: 2em;
      font-weight: bold;
      color: #BE5985;
      margin-bottom: 0;
      margin-top: 0;
      text-shadow: 0 2px 8px #FFEDFA66;
    }
  </style>
</head>
<body>
  <div id="privacy-modal">
    <div id="privacy-modal-content">
      <div id="special-box">
        <h1>Do you want to know what’s waiting for you?</h1>
      </div>
      <h2>For My Love Only 💖</h2>
      <p>Enter your secret code:</p>
      <input type="password" id="secret-code" placeholder="Your code here">
      <button onclick="checkCode()">Enter</button>
      <p id="error-message" style="color:#BE5985"></p>
    </div>
  </div>
  <div class="container" style="display:none;" id="main-content">
    <h1>Happy Birthday, My Love!</h1>
    <div class="love-message">I love you forever! 💖</div>
    <section>
      <label>Wishlist</label>
      <ul id="wishlist">
        <li>Handmade Bracelet</li>
        <li>Romantic Dinner</li>
        <li>Surprise Trip</li>
        <!-- Add more items as you like -->
      </ul>
    </section>
    <section>
      <label>Image</label>
      <img src="YOUR_IMAGE_URL_HERE" alt="Beautiful moment" style="width:100%; border-radius:12px; margin-bottom:8px;">
    </section>
    <section>
      <label>Note</label>
      <div class="note" id="note-content">
        You can write a special note here, babe! 💌
      </div>
      <textarea id="note-input" rows="3" placeholder="Write your note here..." onblur="updateNote()"></textarea>
    </section>
    <section class="music-list">
      <label>Music List</label>
      <ul>
        <li>
          <span>Song 1: Your Favorite Song</span>
          <!-- Example audio embed -->
          <audio controls src="YOUR_SONG_URL.mp3"></audio>
        </li>
        <!-- Add more songs -->
      </ul>
    </section>
    <section>
      <label>Eat List</label>
      <ul>
        <li>Bánh tráng trộn</li>
        <li>Pizza</li>
        <li>Milk Tea</li>
        <!-- Add more foods -->
      </ul>
    </section>
  </div>
  <script>
    // Change this to your secret code
    const SECRET = "16102003";

    function checkCode() {
      const code = document.getElementById('secret-code').value;
      if (code === SECRET) {
        document.getElementById('privacy-modal').style.display = 'none';
        document.getElementById('main-content').style.display = 'block';
      } else {
        document.getElementById('error-message').textContent = "Wrong code! Try again.";
      }
    }
    function updateNote() {
      let note = document.getElementById('note-input').value;
      if (note.trim()) {
        document.getElementById('note-content').textContent = note;
      }
    }
  </script>
</body>
</html>
