
 

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
/* Color fucsia */
body, p, li, h1, h2, h3, h4, h5, h6 {
  color: #ff00ff !important;
}

/* Fuente futurista */
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@300;500;800&display=swap');

h1, h2, h3 {
  font-family: 'Orbitron', sans-serif !important;
  font-weight: 800;
  text-align: center; /* TITULOS CENTRADOS */
  font-size: 34px;    /* MÁS GRANDES */
}

body, p, li {
  font-family: 'Orbitron', sans-serif !important;
  font-weight: 300;
  font-size: 22px;     /* TEXTO MÁS GRANDE */
  line-height: 1.55;   /* MÁS ESPACIADO, MAS LINDO */
  text-align: center;  /* CENTRA TODO EL TEXTO */
}

/* Contenedor centrado como la otra página */
.container {
  max-width: 900px !important; /* como ejemplo que te gustó */
  margin: 0 auto !important;   /* CENTRADO REAL */
  padding: 20px 40px;
  background: transparent !important; /* sin rectángulo gris */
  border: none !important;
  box-shadow: none !important;
}

/* Fondo con GIF en los costados */
body {
  background-color: black;
  background-image:
    url("sudhi-vijay-sudhi-offl.gif"),
    url("sudhi-vijay-sudhi-offl.gif");
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
