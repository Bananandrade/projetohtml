# projeto html
mandar mensagem no whatsapp
<!DOCTYPE html>
<html lang="en">
  <head>
    
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Whatsapp web</title>
    
  
<style>
 @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:ital@1&family=Roboto:wght@100;300&display=swap');
 body{
    display: flex;
  flex-wrap:wrap;
  justify-content:center;
  background-image: url("https://user-images.githubusercontent.com/15075759/28719144-86dc0f70-73b1-11e7-911d-60d70fcded21.png");
   }
  div { 
    background-color:#daf7c1;
    width:320px;
    margin: 8px;
    padding: 8px 18px;
    border-radius: 14px;
    box-shadow: 2px 2px rgba(0, 0, 0, 0.2);
    display:flex;
    justify-content: space-between;
    align-items:center;
  }

  div:hover{
    box-shadow:4px 4px rgba(0, 0, 0,0.4);
    cursor: pointer;
  }
  img{
    width:40px;
    height: 40px;
    border-radius: 50%;
  }
  p{
    font-size:18px;
  }
</style>
  </head>

  <body>
  <div class="card" onclick="mandaZap(this)">
  <p>Bom dia</p>
  <img src="https://i.pinimg.com/originals/d9/d9/7d/d9d97d48264770f85d35c208f279152c.png">
  </div>

  <div class="card" onclick="mandaZap(this)">
  <p>Boa tarde</p>
  <img src="https://i.pinimg.com/originals/d9/d9/7d/d9d97d48264770f85d35c208f279152c.png">
  </div>

  <div class="card" onclick="mandaZap(this)">
  <p>Boa noite</p> 
  <img src="https://i.pinimg.com/originals/d9/d9/7d/d9d97d48264770f85d35c208f279152c.png">
  </div>   
  
  <div class="card" onclick="mandaZap(this)">
  <p>Tudo bem?</p> 
  <img src="https://i.pinimg.com/originals/d9/d9/7d/d9d97d48264770f85d35c208f279152c.png">
  </div>   
  
  <div class="card" onclick="mandaZap(this)">
  <p>O que tá fazendo?</p> 
  <img src="https://i.pinimg.com/originals/d9/d9/7d/d9d97d48264770f85d35c208f279152c.png">
  </div>   
  
  <div class="card" onclick="mandaZap(this)">
  <p>Até mais tarde</p> 
  <img src="https://i.pinimg.com/originals/d9/d9/7d/d9d97d48264770f85d35c208f279152c.png">
  </div>   
              
</div>
 <script>
  function mandaZap(elemento) {
    let texto=elemento.firstElementChild.innerText;
  let numero=prompt("Qual é o número?");
   let zapLink=`https://api.whatsapp.com/send?phone=55${numero}&text=${texto}`;
window.open(zapLink);
  }
   
   </script>
  </body>
</html>
