
<html lang="es">
<head>
    <meta charset="UTF-8"> 
    <title> Planificador de Comidas </title>
    

<link href="https://fonts.googleapis.com/css2?family=Bitcount+Prop+Double:wght@100..900&display=swap" rel="stylesheet">

<style>

body {
font-family: 'Jost';
background-color: red;
 animation-name: fade;
 animation-iteration-count:infinite;
  animation-duration: 5s;
}
@keyframes fade {
 0%   {background-color: rgba(226, 16, 16, 0.871);}
  25%  {background-color: rgb(220, 177, 37);}
  50%  {background-color: rgb(134, 239, 14);}
  75%  {background-color: rgb(11, 227, 177);}
  100% {background-color: rgb(237, 97, 5);}
color:#000000;"
  font-style: normal;
  font-weight: 100 900;
  font-display: swap;
  src: url(https://fonts.gstatic.com/s/jost/v19/92zatBhPNqw73ord4iYl.woff2) format('woff2');
  unicode-range: U+0100-02BA, U+02BD-02C5, U+02C7-02CC, U+02CE-02D7, U+02DD-02FF, U+0304, U+0308, U+0329, U+1D00-1DBF, U+1E00-1E9F, U+1EF2-1EFF, U+2020, U+20A0-20AB, U+20AD-20C0, U+2113, U+2C60-2C7F, U+A720-A7FF;

}

    h1 {
        font-family: 'Bitcount Prop Double';
color:#6d14ea;  
 font-family: "Bitcount Prop Double", system-ui;
  font-optical-sizing: auto;
  font-weight: <weight>;
  font-style: normal;
  font-variation-settings:
  animation-name: "slide";
  animation-duration: 4s;

  
}
input {
color:#370377;  
  font-family: "Playwrite AU QLD", cursive;
  font-optical-sizing: auto;
  font-weight: <weight>;
  font-style: normal;
}


  </style>
  </head> 

   
<center> <h1> BIENVENIDOS A NUESTRA PÁGINA WEB QUE LE AYUDARÁ A ELEGIR SU PRÓXIMO PLATILLO</h1> </center>
<center><link href="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS2975y5Wi7suYu48FfPSEZSmjfRBvPjmsH4g&s">
 </center>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bitcount+Prop+Double:wght@100..900&family=Oswald:wght@200..700&display=swap" rel="stylesheet">


<style>
    p {
font-family: 'Oswald';
  font-style: normal;
  font-weight: 200 700;
  font-display: swap;
  src: url(https://fonts.gstatic.com/s/oswald/v56/TK3iWkUHHAIjg752HT8Ghe4.woff2) format('woff2');
  unicode-range: U+0301, U+0400-045F, U+0490-0491, U+04B0-04B1, U+2116;
}

</style>


<p> DESCRIPCIÓN: Este es un pequeño proyecto en donde tomará en cuenta cuales son sus gustos y basándose en ello le daremos una sugerencia para que pueda elegir con traquilidad y rápidez su platillo  </p>
<span> Llene el siguiente formulario: </span> 
<!-- Formulario -->
<input type="text" id="comidaInput" placeholder="Escriba su platillo favorito aquí">
<style> 
    button {
        color:#000000;  
  font-family: "Playwrite AU QLD", cursive;
  font-optical-sizing: auto;
  font-weight: <weight>;
  font-style: normal;
   background-color: #f5f5f5;
}
</style>
<button onclick="sugerirComida()">Sugerir platos</button>

<!-- Resultado -->
<div id="resultado" style="margin-top: 20px; font-weight: bold;"></div>

<script>
function sugerirComida() {
    // Obtener el valor ingresado
    let comida = document.getElementById("comidaInput").value.toLowerCase();
    let resultado = document.getElementById("resultado");

    // Limpiar contenido previo
    resultado.innerHTML = "";

    // Lógica de recomendación
    if (comida.includes("pizza") || comida.includes("lasagna") || comida.includes("spaghetti") || comida.includes("sopa de tomate")) {
        resultado.innerHTML = "Recomendaciones para ti:<br>🍝 Lasagna<br>🍝 Spaghetti<br>🍲 Sopa de tomate con queso";
    } else if (comida.includes("hamburguesa")) {
        resultado.innerHTML = "Recomendaciones para ti:<br>🍔 Hamburguesa BBQ<br>🍟 Papas con queso<br>🌭 Hot dogs estilo Chicago";
    } else if (comida.includes("ensalada")) {
        resultado.innerHTML = "Recomendaciones para ti:<br>🥗 Ensalada César<br>🥑 Ensalada de aguacate con atún<br>🍅 Tomates rellenos con arroz";
    } else {
        resultado.innerHTML = "Lo siento, aún no tenemos recomendaciones para eso. ¡Prueba con 'pizza', 'hamburguesa' o 'ensalada'!";
    }
}
</script>
</html>
