# Nombre del Proyecto 
Tienda de hardware GAMEFACTOR

## Descripción
Maximiza tu PC: Somos una tienda especializada en componentes de alta calidad para PC. Nuestro objetivo es ayudarte a sacar el máximo potencial de tu computadora. Desde procesadores y tarjetas gráficas hasta unidades de almacenamiento y refrigeración, ofrecemos productos que te permitirán optimizar el rendimiento de tu PC. Además, contamos con expertos en hardware que pueden asesorarte sobre las mejores opciones para tus necesidades específicas. ¡Descubre cómo llevar tu PC al siguiente nivel con nosotros!

## Instalacion
Clona este repositorio:
git clone URL_DEL_REPOSITORIO

Navega al directorio del proyecto:
cd nombre-del-repositorio

Instala las dependencias:
pip install -r requirements.txt

## uso
Ejecuta la aplicación Flask:
python nombre_de_tu_archivo.py

Abre tu navegador y ve a http://127.0.0.1:5000/parts/cpu para ver los datos.

## GF.html
# Tienda de hardware GAMEFACTOR

## Descripción
Maximiza tu PC: Somos una tienda especializada en componentes de alta calidad para PC. Nuestro objetivo es ayudarte a sacar el máximo potencial de tu computadora. Desde procesadores y tarjetas gráficas hasta unidades de almacenamiento y refrigeración, ofrecemos productos que te permitirán optimizar el rendimiento de tu PC. Además, contamos con expertos en hardware que pueden asesorarte sobre las mejores opciones para tus necesidades específicas. ¡Descubre cómo llevar tu PC al siguiente nivel con nosotros!

## GF.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="main.css">
</head>
<body>
<nav>
    <div class="menu">
      <div class="buttoN">
      <ul>
        <li><button class="mostrarINICIO" id="mostrarINICIO">INICIO</button></li>
        <li><button class="mostrar" id="mostrarInfo1">NOSOTROS</button></li>
        <li><button class="mostrar" id="mostrarInfo2">CONTACTO</button></li>
      </ul>
    </div>
    <div id="contenido1" class="contenido"></div>
    <div id="contenido2" class="contenido"></div>
</nav>

<h1 contenteditable data-heading="GAME FACTOR">GAME FACTOR</h1>

<svg id="hs" width="400" height="400" xmlns="http://www.w3.org/2000/svg" overflow="visible">
  <defs>
    <filter id="glow">
      <fegaussianblur class="blur" result="coloredBlur" stddeviation="8"></fegaussianblur>
      <femerge>
        <femergenode in="coloredBlur"></femergenode>
        <femergenode in="coloredBlur"></femergenode>
        <femergenode in="coloredBlur"></femergenode>
        <femergenode in="SourceGraphic"></femergenode>
      </femerge>
    </filter>
    <filter id="filter-broken" filterUnits="objectBoundingBox" x="0" y="0" width="100%" height="100%" color-interpolation-filters="sRGB">
      <feImage preserveAspectRatio="xMidYMid meet" xlink:href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 800 800'%3E%3Crect width='70%25' height='70%25' fill='white'/%3E%3Ccircle cx='50%25' cy='50%25' r='500' %0Afill='none' stroke='black' stroke-width='950' stroke-dasharray='200'/%3E%3C/svg%3E" result="lense"/>
      <feDisplacementMap scale="10" xChannelSelector="B" yChannelSelector="G" in2="lense" in="SourceGraphic" result="disMap"/>
      <feMerge>
        <feMergeNode in="SourceGraphic"/>
        <feMergeNode in="disMap"/>
      </feMerge>
    </filter>
  </defs>
  <style type="text/css">
    #svg_8 { transform-origin: center; }
    svg#hs {
      position: absolute; 
      top: 50%; 
      left: 50%; 
      transform: translate(-50%, -50%); 
      filter: url('#filter-broken');
    }
    #svg_12 {
      filter: url('#filter-broken') url('#glow');
      mix-blend-mode: multiply;
      transform-origin: center;
    }
    .path {
      animation: animation1 3s ease-in-out 1s infinite alternate;
      fill-opacity: .25;
      transform-origin: center;
    }
    .p_0 {
      animation: animation2 3s ease-in-out .5s infinite alternate;
      transform-origin: center;
    }
    @keyframes animation1 {
      from { transform: perspective(400px) rotateX(20deg); }
      to { transform: perspective(400px) rotateX(-20deg); }
      from { transform: perspective(400px) rotateY(20deg); }
      to { transform: perspective(400px) rotateY(-20deg); }
      from { stroke-width: 1; }
      to { stroke-width: 9; }
    }
  </style>
</svg>

<script src="red.js"></script>
<script src="second.js"></script>
<script src="contact.js"></script>
</body>
</html>


## main.css
/* Estilos existentes */
menu {
	display: flex;
	padding: 0;
	margin: 0;
  }
  
  ul {
	display: flex;
	justify-content: center;
  }
  
  .menu li {
	margin-left: 100px;
	display: flex;
	justify-content: center;
	align-items: center; 
  }
  
  .button {
	padding: 0;
	margin: 0;
	justify-content: flex-start;
	border-bottom: #800080;
  }
  
  .mostrarINICIO {
	font-size: 45px;
  }
  
  .mostrar {
	font-size: 45px;
  }
  
  #results {
	margin-top: 20px;
  }
  
  .scrollable {
	width: 300px;
	height: 200px;
	overflow-y: scroll; /* Habilita el scroll vertical */
	border: 1px solid #ccc;
	padding: 10px;
  }
  
  buttoN {
	background-color: transparent;
	border-color: transparent;
	font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
	font-style: italic;
	padding: 0;
	margin: 0;
	color: aquamarine;
	cursor: pointer;
	gap: 25px;
  }
  
  body { 
	overflow: hidden;
	height: 100vh;
	width: 100vw;
	background: linear-gradient(#34046b, #800080);
  }
  
  h1 {
	text-align: center;
	font-size: 14vw;
	position: relative;
	font-weight: 900;
	text-transform: uppercase;
	line-height: 1;
	top: -25;
	color: transparent;
  }
  
  h1::before, h1::after {
	content: attr(data-heading);
	position: absolute;
	top: 0;
	left: 0;  
  }
  
  h1::before {
	color: #3700ff;
	clip-path: polygon(0% 100%, 100% 100%, 100% 40%,  60%);
  }
  
  h1::after {
	color: #800080;
	clip-path: polygon(0 0, 100% 0%, 100% 36%,  56%);
	animation: slide 5s infinite;
  }
  
  @keyframes slide {
	0% {
	  transform: translateX(0);
	}
	20% {
	  transform: translate(-20px, 2%);
	}
  }
  
  /* Estilos responsivos */
  @media (max-width: 768px) {
	.menu li {
	  margin-left: 20px; /* Reduce el margen en pantallas más pequeñas */
	}
  
	.mostrarINICIO, .mostrar {
	  font-size: 24px; /* Reduce el tamaño de fuente en pantallas más pequeñas */
	}
  
	.scrollable {
		overflow-y: scroll;
	  width: 100%; /* Ajusta el ancho al 100% del contenedor */
	  height: 150px; /* Ajusta la altura en pantallas más pequeñas */
	}
  
	h1 {
	  font-size: 10vw; /* Ajusta el tamaño de fuente del título */
	}
  }

  ## image.png
imagen asosciada a la API

## archivo

## API.js
document.getElementById('fetchData').addEventListener('click', () => {
    fetch('http://127.0.0.1:5000/parts/cpu', {
        method: 'GET',
        headers: {
            'Content-Type': 'application/json'
        },
        mode: 'cors'
    })
    .then(response => {
        if (!response.ok) {
            throw new Error('Network response was not ok');
        }
        return response.json();
    })
    .then(data => {
        console.log(data);  // Verificar los datos en la consola
        const resultsDiv = document.getElementById('results');
        
        // Limpiar el contenido anterior
        resultsDiv.innerHTML = '';

        // Mostrar la estructura de los datos en la página
        resultsDiv.textContent = JSON.stringify(data, null, 2);
    })
    .catch(error => console.error('Error:', error));
});

## app.py
(archivo necesario para el correcto funcionamiento de la API)
from flask import Flask, jsonify
from flask_cors import CORS

app = Flask(__name__)
CORS(app)  # Habilita CORS para todas las rutas

@app.route('/parts/cpu')
def get_cpu_parts():
    data = {
        "brand": "Intel",
        "model": "Core i9-9900K",
        "cores": 8,
        "base_clock": 3.6,
        "boost_clock": 5.0,
        "tdp": 95,
        "integrated_graphics": "Intel UHD Graphics 630",
        "multithreading": True,
        "price": 499.99
    }
    return jsonify(data)

if __name__ == '__main__':
    app.run(debug=True)

## function.py
(Archivo complemento para la correcta syntaxis de la API en el servidor flask)
import asyncio

def get_or_create_eventloop():
    try:
        return asyncio.get_event_loop()
    except RuntimeError:
        loop = asyncio.new_event_loop()
        asyncio.set_event_loop(loop)
        return loop

## requirements.txt
(Archivo .txt necesario para la utilización de flask y request 
y necesario para cumplir con las politicas del servidor)

flask
requests

## app.js
(script de efecto y ajuste para el svg)

function init() {
  var timeline = anime.timeline({
    direction: 'alternate',
    easing: 'easeInOutQuint',
    autoplay: true,
    duration: function() {
      return anime.random(0, 270);
    },
    delay: [45, 250],
    loop:true,
  });
  timeline.add({
    targets: ['feDisplacementMap'],
    scale:[5 , 30, 10]
  });
  timeline.add({
    targets: ['#svg_8'],
    fill: ['#150485', '#590995', '#c62a88', '#03c4a1'],
    scale: [.5, 1.05],
    complete: init
  });

  var stroke_anim1 = anime({
    targets: ['#svg_12'],
    strokeDashoffset: [anime.setDashoffset, 0],
    points: [
      { value: [
        '88.5,80.45313l272.5,79.54688l-231,189l-41.5,-268.54688z',
        '207.5,185.45313l156.5,-26.45313l,190l-44.5,-268.54687z'], duration:20000,
      },
    ],
    fill: ['#150485', '#590995', '#c62a88', '#03c4a1'],
    stroke: ['#f1e7b6', '#fe346e', '#400082', '#00bdaa'],
    easing: 'easeOutQuad',
    duration: 2000,
    autoplay:true,
    loop: true,
  });
};

init();

  var rotate_stroke_anime = anime({
    targets: ['#svg_13 path' ],
    easing: ['easeOutInCirc'],
    strokeDashoffset:  [10, 0],
    duration: 1000,
    opacity:.5,
    skewY:100,
    skewX:100,
    rotate:[45, 90],
    autoplay:true,
    direction:'normal',
    loop: true,
    stroke:[.3, 1],
    stroke: ['#150485', '#590995', '#c62a88', '#03c4a1'],

  });

  window.addEventListener("scroll", function(){
    var ul = document.querySelector("ul");
    ul.classList.toggle("abajo", window.scrollY>0);
  })

## red.js
(scrpit para redirijir dando clic al boton INICIO)
document.getElementById("mostrarINICIO").addEventListener("click", function() {
    window.location.href = "GF.html"; 
});

  
## second.js
(script para dar función en el boton NOSOTROS)
function showhide(id, content) {
    var div = document.getElementById(id);
    div.innerHTML = content;
    div.style.display = div.style.display === "none" ? "block" : "none";
}

document.getElementById("mostrarInfo1").addEventListener("click", function() {
    showhide("contenido1", '<span style="font-size: 24px; color:white;">En GAME FACTOR, somos apasionados por la tecnología y el rendimiento. Desde nuestros inicios, hemos tenido una misión clara: proporcionar a nuestros clientes todo lo necesario para llevar sus PCs al siguiente nivel.</span>');
});

## contact.js 
(script para dar función en el boton CONTACTO)
document.getElementById("mostrarInfo2").addEventListener("click", function() {
    var element = document.getElementById("contenido2");
    if (element.style.display === "none") {
        element.innerHTML = `
            <span style="font-size: 24px; color:white;">📞5510821711</span><br>
            <span style="font-size: 24px; color:white;">📞5523497865</span><br>
            <span style="font-size: 24px; color:white;">📩GF/la</span><br>
            <span style="font-size: 24px; color:white;">©GF.es 2024</span>
        `;
        element.style.display = "block";
    } else {
        element.style.display = "none";
    }
});

## contribuir
Contribuir
Haz un fork del repositorio.
Crea una nueva rama:
git checkout -b mi-rama

Haz tus cambios y haz commit:
git commit -m "Descripción de los cambios"

Envía tus cambios:
git push origin mi-rama

Abre un Pull Request.

## Licencia
Este proyecto está bajo la licencia MIT.