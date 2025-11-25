

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
body, p, li, h1, h2, h3, h4, h5, h6 {
  color: #ff00ff !important;
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
header h1 {
  display: none !important;
}  

.container {
  background-color: #1a1a1a;
  padding: 20px;
}
</style>

<style>
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

/* media query aparte */
@media (min-width: 1200px) {
  body {
    padding-left: 200px;
    padding-right: 200px;
  }
}
</style>


<style>
.container {
  max-width: 900px !important;           /* el mismo tamaño que tu página de instalación */
  margin-left: auto !important;
  margin-right: auto !important;
  background-color: rgba(0,0,0,0.85);
  padding: 30px;
  border-radius: 8px;
  z-index: 2;
  position: relative;
  text-align: left !important;           /* MUY IMPORTANTE: texto alineado a la izquierda */
}
</style>


<style>

* {
  font-size: 24px !important;  
}
</style>


