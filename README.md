<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <title>Proposta di San Valentino</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 50px;
      background: #fefefe;
    }
    h1 {
      font-size: 2em;
      color: #c0392b;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 16px;
      cursor: pointer;
    }
    #response {
      margin-top: 30px;
      font-size: 1.2em;
      color: #34495e;
    }
  </style>
</head>
<body>
  <h1>¿Querés ser mi san valentin?</h1>
  <div>
    <button id="yesBtn">Si</button>
    <button id="noBtn">No</button>
  </div>
  <p id="response"></p>
  
  <script>
    let noCount = 0;
    const response = document.getElementById("response");
    
    document.getElementById("yesBtn").addEventListener("click", function(){
      response.textContent = "yeyeyey gachassss mi niña me haces feliz♥️ (sabia que ibas a decir que si ehehehe😌)";
    });
    
    document.getElementById("noBtn").addEventListener("click", function(){
      noCount++;
      if(noCount === 1) {
        response.textContent = "ay nuuu porque?";
      } else if(noCount === 2) {
        response.textContent = "que mala...";
      } else if(noCount === 3) {
        response.textContent = "está bien no me queres ya vi🥺";
      } else if(noCount === 4) {
        response.textContent = "no me importa, estás obligada a decir que si, así que apreta el otro botón graciasssss😌🔪";
      }
    });
  </script>
</body>
</html>
