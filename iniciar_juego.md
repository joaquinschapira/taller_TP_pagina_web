
<a href="index.html" class="btn-volver">⟵ Volver</a>

<style>
.btn-volver {
  position: fixed;
  top: 20px;
  left: 20px;
  background: #ff00ff;
  color: black !important;
  padding: 10px 18px;
  font-size: 20px;
  font-weight: 600;
  border-radius: 8px;
  text-decoration: none;
  font-family: 'Orbitron', sans-serif;
  z-index: 9999;
  transition: 0.2s ease-in-out;
}

.btn-volver:hover {
  background: #ff55ff;
  transform: scale(1.05);
}
</style>


# Iniciar el Juego

### 🖥️ Iniciar el servidor

Primero, se debe crear el servidor al que se conectarán los jugadores:

./needforspeed2d.sh run server


### 🚗 Iniciar un cliente

Cada jugador que quiera jugar debe ejecutar:

./needforspeed2d.sh run client


Al hacerlo se abrirá una ventana simple e intuitiva con dos opciones:

- **Crear Partida**
- **Unirse a Partida**

---

## Crear Partida

Si elegís **Crear Partida**, serás el anfitrión. Podrás:

- Elegir tu **nombre**.
- Seleccionar tu **auto**.
- Elegir uno o más **mapas jugables** creados en el editor.  
  > *Si aún no creaste mapas, volvé a la sección del **[Editor de Mapas](#editor-de-mapas)**.

Al confirmar, se abrirá la ventana de **pre-partida/lobby**, donde se generará un **código de 4 dígitos**.  
Los demás jugadores deberán usar ese código para unirse.

---

## Unirse a Partida

Si elegís **Unirse a Partida**, deberás:

1. Escribir tu **nombre**.  
2. Elegir tu **auto**.  
3. Introducir el **código de partida** que brinda el anfitrión.

Después de aceptar, ingresarás a la **pre-partida/lobby**.

---

## Pre-partida / Lobby

En esta sala de espera:

- Los jugadores aparecerán con su nombre y auto.  
- Cuando todos estén listos, podrán comenzar la partida.

---


<style>
/* Títulos bien fucsia */
h1, h2, h3, h4, h5, h6 {
  color: #ff00ff !important;
}

 
body, p, li {
  color: #ffddff !important;
}
</style>

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
/* Fondo general con GIFs a los costados */
body {
  background-color: black;
  background-image:
    url("sudhi-vijay-sudhi-offl.gif"),
    url("sudhi-vijay-sudhi-offl.gif");
  background-repeat: repeat-y;
  background-position:
    left center,
    right center;
  background-size: 200px; 
}

@media (min-width: 1200px) {
  body {
    padding-left: 200px;
    padding-right: 200px;
  }
}


header h1 {
  display: none !important;
}

/* Container centrado tipo “tarjeta” de lectura */
.container {
  max-width: 900px !important;          
  margin-left: auto !important;
  margin-right: auto !important;
  background-color: rgba(0,0,0,0.85);
  padding: 30px;
  border-radius: 8px;
  z-index: 2;
  position: relative;
  text-align: left !important;
}
</style>

<style>
/* Tamaños de fuente */
body {
  font-size: 20px;
}

p, li {
  font-size: 22px;
}

h1 {
  font-size: 40px !important;
}

h2 {
  font-size: 32px !important;
}

h3 {
  font-size: 26px !important;
}
</style>

<style>
/* Estilo terminal para los comandos */
.command {
  display: block;
  background: #111;
  border-left: 4px solid #ff00ff;
  padding: 8px 12px;
  margin: 8px 0 12px 0;
  font-family: "Fira Code", monospace;
  font-size: 20px;
  color: #ffddff;
  border-radius: 6px;
}
</style>

<style>

a[href*="github.com"][class*="btn"],
.page-header a.btn,
header a.btn,
.btn[href*="github"] {
  display: none !important;
}


.page-header {
  display: none !important;
}
</style>