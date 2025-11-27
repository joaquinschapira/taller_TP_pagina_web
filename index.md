<div class="titulo-grande">NEED FOR SPEED 2D</div>




<div class="hero-inicio"></div>

<div class="menu-botones">
  <a class="boton-fucsia" href="como_se_juega.html">¿Cómo se juega?</a>
  <a class="boton-fucsia" href="instalar_compilar.html">¿Cómo instalar, compilar y ejecutar?</a>
  <a class="boton-fucsia" href="iniciar_juego.html">¿Cómo iniciar una partida? </a>
</div>



<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@300;500;800&display=swap');

h1, h2, h3 {
  font-family: 'Orbitron', sans-serif !important;
  font-weight: 800;
}

body, p, li {
  font-family: 'Orbitron', sans-serif !important;
  font-weight: 300;
}
</style>


<style>
header h1 {
  display: none !important;
}
</style>

<style>
/* Títulos y cosas importantes */
h1, h2, h3, h4, h5, h6 {
  color: #ff00ff !important;
}

/* Texto normal un poco más suave */
body, p, li {
  color: #ffddff !important;
}
</style>

 
<style>

.container {
  background-color: #1a1a1a;
  padding: 20px;
}
</style>

<style>





body {
  background-color: black;
  background-image:
    url("gif.gif"),
    url("gif.gif");
  background-repeat: repeat-y;
  background-position:
    left center,
    right center;
  background-size: 180px; 

}
@media (min-width: 1200px) {
  body {
    padding-left: 200px;
    padding-right: 200px;
  }
}

</style>
 

---





<div class="video-container">
  <video controls width="800">
    <source src="video_juego.mp4" type="video/mp4">
    Tu navegador no soporta el video HTML5.
  </video>
</div>

 <img src="racecar.jpg" alt="foto" style="float:right; width:260px; margin: 10px; border: 2px solid #ff00ff;">




<style>
.menu-botones {
  text-align: center;
  margin-bottom: 25px;
}

.boton-fucsia {
  display:inline-block;
  padding:10px 20px;
  background:#ff00ff;
  color:black !important;
  font-weight:bold;
  border-radius:10px;
  text-decoration:none;
  margin:8px;
  border: 2px solid #ffffff33;
  box-shadow: 0 0 10px rgba(255,0,255,0.5);
  transition: transform 0.15s ease, box-shadow 0.15s ease, background 0.15s ease;
}

.boton-fucsia:hover {
  transform: translateY(-2px);
  box-shadow: 0 0 18px rgba(255,0,255,0.9);
  background:#ff55ff;
}
</style>

<style>
.container {
  max-width: 1200px !important;   /* antes estaba en 900px */
  margin: auto;
  background-color: rgba(0,0,0,0.85);
  padding: 30px;
  border-radius: 8px;
  z-index: 2;
  position: relative;
}
</style>

<style>
body {
  font-size: 20px;
}

p, li {
  font-size: 22px;
}
</style>

<style>
.titulo-grande {
  font-size: 120px !important;   
  line-height: 0.9;
}
</style>


<style>
.banner-superior img {
  width: 100%;
  height: auto;
  display: block;
  margin: 0;
  padding: 0;
}
</style>


<style>
.titulo-grande {
  font-family: 'Orbitron', sans-serif !important;
  font-weight: 800;
  font-size: 150px;              /* tamaño gigante */
  color: #ff00ff !important;    /* tu fucsia */
  text-align: center;           /* centrado */
  margin-top: 40px;
  margin-bottom: 50px;
  letter-spacing: 3px;          /* un toque más futurista */
  text-shadow: 0 0 10px #ff00ff, 
               0 0 20px #ff00ff;
}
@media (max-width: 768px) {
  .titulo-grande {
    font-size: 45px;            /* más chico en celulares */
  }
}
</style>



Este juego ha sido desarrollado por los alumnos: Lucas Pagani, Federico Zanor, Manuel Pato y Joaquin Schapira como trabajo practico final para la materia taller de programación en la facultad de ingenieria de la UBA. El trabajo consistia en desarrollar el mítico juego need for speed 2d permitiendo el multijugador para aplicar todo lo aprendido en la materia. 


<div class="integrantes-container">

  <div class="integrante">
    <div class="integrante-nombre">Lucas Pagani</div>
    <a class="integrante-github" href="https://github.com/USUARIO1" target="_blank">GitHub</a>
  </div>

  <div class="integrante">
    <div class="integrante-nombre">Federico Zanor</div>
    <a class="integrante-github" href="https://github.com/USUARIO2" target="_blank">GitHub</a>
  </div>

  <div class="integrante">
    <div class="integrante-nombre">Manuel Pato</div>
    <a class="integrante-github" href="https://github.com/USUARIO3" target="_blank">GitHub</a>
  </div>

  <div class="integrante">
    <div class="integrante-nombre">Joaquin Schapira</div>
    <a class="integrante-github" href="https://github.com/USUARIO4" target="_blank">GitHub</a>
  </div>

</div>



<style>
.titulo-grande {
  font-family: 'Orbitron', sans-serif !important;
  font-weight: 800;
  text-align: center;

  font-size: 160px !important;    /* TAMAÑO GRANDE */
  color: #ff00ff;

  letter-spacing: 6px;
  margin-top: 40px;
  margin-bottom: 40px;

  /* NEÓN TRIPLE */
  text-shadow:
    0 0 8px #ff00ff,
    0 0 16px #ff00ff,
    0 0 32px #ff00ff,
    0 0 48px #ff66ff,
    0 0 72px #ff99ff;

  /* BORDE EXTERNO */
  -webkit-text-stroke: 3px #770077;

  /* ANIMACIÓN SUAVE */
  animation: pulso-neon 2.5s infinite ease-in-out;
}

@keyframes pulso-neon {
  0%, 100% {
    text-shadow:
      0 0 8px #ff00ff,
      0 0 16px #ff00ff,
      0 0 32px #ff00ff,
      0 0 48px #ff66ff,
      0 0 72px #ff99ff;
  }
  50% {
    text-shadow:
      0 0 4px #ff00ff,
      0 0 12px #ff00ff,
      0 0 20px #ff00ff,
      0 0 30px #ff66ff,
      0 0 40px #ff99ff;
  }
}

@media (max-width: 768px) {
  .titulo-grande {
    font-size: 70px !important;
    -webkit-text-stroke: 1px #770077;
  }
}
</style>

<style>
.video-container {
  text-align: center;
  margin: 30px 0;
}

.video-container video {
  max-width: 100%;
  border: 3px solid #ff00ff;
  border-radius: 10px;
  box-shadow: 0 0 25px rgba(255,0,255,0.6);
}
</style>

<div class="boton-grande-container">
  <a class="boton-grande" href="https://github.com/lucasPagani2003/taller-de-programacion-tp-grupal-2025c2-grupo-2" target="_blank">
    🔗 Ver repositorio en GitHub
  </a>
</div>


<style>
.boton-grande-container {
  text-align: center;
  margin: 50px auto 30px auto;
}

.boton-grande {
  display: inline-block;
  padding: 18px 40px;
  font-size: 32px;     /* MÁS GRANDE */
  font-weight: 800;
  font-family: 'Orbitron', sans-serif !important;

  background: #ff00ff;
  color: black !important;
  text-decoration: none;
  border-radius: 12px;

  border: 3px solid #ffffff55;
  box-shadow: 0 0 20px rgba(255,0,255,0.6);
  letter-spacing: 2px;

  transition: transform 0.2s ease, box-shadow 0.2s ease, background 0.2s ease;
}

/* EFECTO HOVER */
.boton-grande:hover {
  transform: translateY(-3px) scale(1.05);
  background: #ff55ff;
  box-shadow: 0 0 30px rgba(255,0,255,0.95);
}
</style>


<style>

/* Contenedor principal: 4 columnas */
.integrantes-container {
  display: flex;
  justify-content: center;
  gap: 40px;
  margin-top: 60px;
  margin-bottom: 80px;
  flex-wrap: wrap; 
}

/* Cada integrante */
.integrante {
  text-align: center;
  width: 220px;
  background: rgba(0,0,0,0.6);
  padding: 20px 15px;
  border-radius: 15px;
  box-shadow: 0 0 25px rgba(255,0,255,0.4);
  border: 2px solid #ff00ff55;
}

/* Nombre */
.integrante-nombre {
  font-family: 'Orbitron', sans-serif !important;
  font-size: 26px;
  font-weight: 800;
  color: #ff00ff;
  margin-bottom: 15px;
  text-shadow: 0 0 10px #ff00ff;
}

/* Botón GitHub */
.integrante-github {
  display: inline-block;
  padding: 10px 20px;
  background: #ff00ff;
  color: black !important;
  font-weight: bold;
  text-decoration: none;
  border-radius: 8px;
  border: 2px solid #ffffff33;
  box-shadow: 0 0 15px rgba(255,0,255,0.7);
  transition: transform 0.15s ease, box-shadow 0.15s ease, background 0.2s ease;
}

.integrante-github:hover {
  transform: translateY(-3px) scale(1.05);
  background: #ff55ff;
  box-shadow: 0 0 25px rgba(255,0,255,1);
}


@media (max-width: 780px) {
  .integrante {
    width: 100%;
    max-width: 350px;
  }
}

</style>



<style>

/* Tamaño general del texto (mucho más razonable) */
body {
  font-size: 14px !important;
}

p, li {
  font-size: 15px !important;
}

/* Títulos más chicos */
h1 {
  font-size: 28px !important;
}
h2 {
  font-size: 24px !important;
}
h3 {
  font-size: 20px !important;
}
h4, h5, h6 {
  font-size: 18px !important;
}

/* Botones */
.boton-fucsia {
  font-size: 16px !important;
}

/* Botón gigante del GitHub */
.boton-grande {
  font-size: 22px !important;
  padding: 12px 28px !important;
}

/* Integrantes */
.integrante-nombre {
  font-size: 20px !important;
}
.integrante-github {
  font-size: 16px !important;
}

/* EL TÍTULO PRINCIPAL — mucho más razonable */
.titulo-grande {
  font-size: 70px !important;
  -webkit-text-stroke: 2px #770077 !important;
}


@media (max-width: 768px) {
  .titulo-grande {
    font-size: 40px !important;
    -webkit-text-stroke: 1px #770077 !important;
  }
}

</style>