

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

# Cómo se juega

## 🕹️ Manual del Juego

Antes de comenzar a jugar, es importante saber que **el juego funciona exclusivamente con mapas creados por el usuario**.  
Si es tu primera vez, deberás abrir el **editor interactivo** y diseñar tus propios mapas.

Si ya tenés mapas creados o sabés usar el editor, podés saltar a la sección **[Iniciar el Juego](#iniciar-el-juego)**.

---

## Editor de Mapas

Para abrir el editor, ejecutá:

<code class="command">./needforspeed2d.sh run editor</code>


Dentro del editor podrás elegir una de las siguientes **tres ciudades base**:

- **San Andreas**: grandes avenidas y rectas ideales para alcanzar altas velocidades.  
- **Vice City**: calles estrechas y cortas, perfectas para poner a prueba el control del auto.  
- **Liberty City**: un gran río, una isla central y puentes que conectan toda la ciudad.

### 🧱 Colocación de elementos

En la barra superior podrás seleccionar qué colocar en el mapa:

- **Salida**
- **Meta**
- **Checkpoint(s)**

El cursor mostrará el objeto seleccionado e indicará si su posición es válida o no.  
Tené en cuenta:

- La **salida** ocupa mucho espacio y puede costar ubicarla.  
- La **meta** y los **checkpoints** son más permisivos y se adaptan a las celdas disponibles. 

Además, tanto la **salida** como los **checkpoints** pueden ser rotados si se presiona la tecla **R**. 
La salida mostrará una flecha en la dirección en la que saldrán los autos.

Si cometés un error:

- Usá la opción **"Borrar"** y hacé clic en el objeto a eliminar.
- Podés usar **"Deshacer"** o presionar **Ctrl + Z**.

### 💾 Guardado de mapas

Cuando termines, deberás **guardar tu mapa como jugable** usando:

- **Guardar como…** → permite asignar un nombre al nuevo mapa.  
- **Abrir Mapa Jugable** → para modificar un mapa ya existente.  
- **Guardar** → actualiza un mapa previamente creado.

---


<style>
/* Títulos bien fucsia */
h1, h2, h3, h4, h5, h6 {
  color: #ff00ff !important;
}

/* Texto un poco más suave para que no canse */
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
    url("art pixel GIF.gif"),
    url("art pixel GIF.gif");
  background-repeat: repeat-y;
  background-position:
    left center,
    right center;
  background-size: 200px;
}

/* Para pantallas grandes sumo padding lateral */
@media (min-width: 1200px) {
  body {
    padding-left: 200px;
    padding-right: 200px;
  }
}

/* Ocultar título del theme */
header h1 {
  display: none !important;
}

/* Container centrado tipo “tarjeta” de lectura */
.container {
  max-width: 900px !important;        /* perfecto para texto */
  margin: 0 auto;
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