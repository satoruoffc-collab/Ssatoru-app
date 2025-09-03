<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<title>Satoru App</title>
<style>
  body { margin:0; font-family: Arial, sans-serif; text-align:center; color:white; }
  .page { display:none; padding:20px; }
  .active { display:block; }
  body.login { background-color:#222; }
  body.satoru { 
    background-image: url('https://i.postimg.cc/SsPvsyfj/7bbfcafd-3fc2-49cf-81b9-ba85535a6927.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
  }
  input, button { padding:10px; margin:5px; font-size:16px; }
</style>
</head>
<body class="login">

<!-- Login Seite -->
<div id="loginPage" class="page active">
  <h2>Login</h2>
  <input type="text" id="username" placeholder="Benutzername"><br>
  <input type="password" id="password" placeholder="Passwort"><br>
  <button onclick="checkLogin()">Einloggen</button><br><br>
  <button onclick="alert('Zugang freischalten')">Zugang freischalten</button>
</div>

<!-- Satoru Seite -->
<div id="satoruPage" class="page">
  <h1 style="color:red;">Satoru wird Siegen</h1>
  <h3 style="color: darkgreen; text-shadow: 0 0 5px limegreen,0 0 10px limegreen,0 0 20px green;">Dont play with death☢️☝🏻</h3>
  <h4 style="color:red">betet zu Satoru</h4>
  <button onclick="showPage('nummerPage')">Virus send to +49XXXXXX</button><br>
  <button>Ban Checker</button><br><br>
  <button onclick="showPage('thanksPage')">THANKS TO</button><br><br>
  <p><a href="https://t.me/NevErl0seU013" target="_blank">Contact me</a></p>
  <p><a href="https://www.paypal.com/MaxBauer705" target="_blank"><strong>Buy premium</strong></a></p>
  <h3 style="color:red;">Gefallen für ein Mädchen auferstanden für meine Jungs</h3>
  <h1>Fucked by Satoru</h1>
</div>

<!-- Telefonnummer Seite -->
<div id="nummerPage" class="page">
  <h1>49😈😈😈😈</h1>
  <input type="tel" id="telefon" placeholder="Telefonnummer"><br>
  <button onclick="alert(document.getElementById('telefon').value)">send..</button><br><br>
  <button onclick="showPage('satoruPage')">ZURÜCK</button>
</div>

<!-- Thanks Seite -->
<div id="thanksPage" class="page">
  <h1>SATORU</h1>
  <h6><strong>THANKS TO</strong></h6>
  <h1>1. ARES mein Bruder</h1>
  <h2>2. C1DRIP auch mein Bruder</h2>
  <h1>3. NIKKI mein erster Mentor und auch mein Bruder</h1>
  <button onclick="showPage('satoruPage')">ZURÜCK</button>
</div>

<script>
function checkLogin() {
  var user = document.getElementById('username').value.trim();
  var pass = document.getElementById('password').value.trim();
  if(user === 'satoru' && pass === 'satoru0132'){
    document.body.className = 'satoru';
    showPage('satoruPage');
  } else {
    // Fallback-Link bei falschem Login
    window.location.href = 'https://www.google.com';
  }
}

function showPage(pageId){
  var pages = document.querySelectorAll('.page');
  pages.forEach(function(p){ p.classList.remove('active'); });
  document.getElementById(pageId).classList.add('active');
}
</script>

</body>
</html># Ssatoru-app
