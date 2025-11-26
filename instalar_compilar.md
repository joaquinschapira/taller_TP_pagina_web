# 🔧 Instalación, Compilación y Ejecución

Antes de jugar, es necesario instalar las dependencias y compilar el proyecto.  
No se necesita conocimiento alguno de C++: todo está automatizado mediante el script `needforspeed2d.sh`.

---

## 1° Requisitos del Sistema

- Sistema operativo compatible:
  - Ubuntu 24.04 (o distribuciones Linux derivadas)

---

## 2° Otorgar permisos de ejecución

<code class="command">chmod +x needforspeed2d.sh</code>

---

## 3° Descargar dependencias

Este comando instala todas las librerías necesarias (SDL, Qt, cmake, etc.):

<code class="command">sudo ./needforspeed2d.sh download</code>

---

## 4° Compilar proyecto

**Compilación normal:**
<code class="command">./needforspeed2d.sh build</code>

**Compilación limpia:**
<code class="command">./needforspeed2d.sh build --clean</code>
<code class="command">./needforspeed2d.sh build --c</code>

---

## 5° Ejecutar tests

<code class="command">./needforspeed2d.sh tests</code>

---

## 6° Ejecutar

El proyecto incluye tres ejecutables:

- Cliente
- Servidor
- Editor de mapas

Todo se ejecuta desde el instalador:

Cliente:
<code class="command">./needforspeed2d.sh run client</code>

Servidor:
<code class="command">./needforspeed2d.sh run server</code>

Editor:
<code class="command">./needforspeed2d.sh run editor</code>

---

## 7° Ejecutar con Valgrind (opcional)

Importante:

- Cliente y Editor usan Valgrind_helpers para supresiones (ver markdown de ese directorio).
- Server no usa supresiones.

Cliente:
<code class="command">./needforspeed2d.sh run client --valgrind</code>

Servidor:
<code class="command">./needforspeed2d.sh run server --valgrind</code>

Editor:
<code class="command">./needforspeed2d.sh run editor --valgrind</code>

---

## 8° Configuración del software

El archivo de configuración se encuentra en:

<code class="command">etc/need4speed/config.yaml</code>

Permite modificar duración de carrera, características de autos, tiempos de pantallas intermedias y más.  
No es necesario modificarlo para jugar.

Los recursos utilizados (mapas, texturas, sonidos) se encuentran en:

<code class="command">resources/</code>

Ya vienen listos al compilar.

---

<style>
/* Títulos bien fucsia */
h1, h2, h3, h4, h5, h6 {
  color: #ff00ff !important;
}

/* Texto más suave */
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
/* Fondo general */
body {
  background-color: black;
  background-image:
    url("auto.gif"),
    url("auto.gif");
  background-repeat: repeat-y;
  background-position:
    left center,
    right center;
  background-size: 200px;
}

/* Padding lateral en pantallas grandes */
@media (min-width: 1200px) {
  body {
    padding-left: 200px;
    padding-right: 200px;
  }
}

/* Ocultar título del tema */
header h1 {
  display: none !important;
}

/* Container estilo tarjeta */
.container {
  max-width: 900px !important;
  margin: 0 auto;
  background-color: rgba(0,0,0,0.85);
  padding: 30px;
  border-radius: 8px;
  z-index: 2;
  position: relative;
  text-align: left !important;
}
</style>

<style>
/* Tamaños coherentes */
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
/* Comandos estilo terminal */
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
