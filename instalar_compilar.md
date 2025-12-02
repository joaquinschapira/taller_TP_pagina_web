
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

🔧 Instalación, Compilación y Ejecución

Antes de utilizar el juego, es necesario instalar las dependencias y compilar el proyecto.
Todo el proceso está automatizado mediante el script needforspeed2d.sh.

1° Requisitos del Sistema

Sistema operativo compatible:

Ubuntu 24.04 o distribuciones Linux derivadas.

2° Clonar el repositorio

<code class="command">git clone https://github.com/lucasPagani2003/taller-de-programacion-tp-grupal-2025c2-grupo-2.git

</code>

3° Instalar el proyecto

Este paso debe ejecutarse como root, ya que instala binarios y copia assets/config.

<code class="command">sudo ./needforspeed2d.sh install</code>

¿Qué hace internamente?

Instala dependencias esenciales

Compila el proyecto

Ejecuta los tests del protocolo

Instala los ejecutables en el sistema:

/usr/bin/taller_client

/usr/bin/taller_server

/usr/bin/taller_editor

Copia recursos del juego a /var/need4speed

Copia configuración a /etc/need4speed

Los mapas jugables se guardan en:

<code class="command">~/.local/share/need4speed/mapas_jugables</code>

Los archivos de configuración permiten ajustar duración de carrera, características de autos, tiempos de pantallas, etc.
No es necesario modificar nada para jugar.

4° Descargar dependencias (solo desarrolladores)

Solo necesario si agregás nuevas librerías al proyecto.

Instala SDL, Qt, CMake y todas las dependencias:

<code class="command">sudo ./needforspeed2d.sh download</code>

5° Compilar manualmente (solo desarrolladores)

Compilación normal:

<code class="command">sudo ./needforspeed2d.sh build</code>

Compilación limpia:

<code class="command">sudo ./needforspeed2d.sh build --clean</code>
<code class="command">sudo ./needforspeed2d.sh build --c</code>

6° Ejecutar tests manualmente

Debe ejecutarse desde la raíz del repositorio:

<code class="command">sudo ./needforspeed2d.sh tests</code>

7° Ejecutar el proyecto

El sistema incluye tres ejecutables:

Cliente

Servidor

Editor de mapas

Si el proyecto fue instalado (Inciso 3):

Editor:
<code class="command">taller_editor</code>

Servidor:
<code class="command">taller_server 8080</code>

Cliente:
<code class="command">taller_client localhost 8080</code>

Si NO se instaló pero sí se descargaron dependencias y compiló manualmente:

Cliente:
<code class="command">./needforspeed2d.sh run client</code>

Servidor:
<code class="command">./needforspeed2d.sh run server</code>

Editor:
<code class="command">./needforspeed2d.sh run editor</code>

8° Ejecutar con Valgrind (opcional)

Cliente y editor utilizan Valgrind_helpers para supresiones.
Qt y SDL tienen algunos errores no suprimibles pero no afectan al proyecto.
El servidor no requiere supresiones.

Desde la raíz del repositorio:

Cliente:
<code class="command">./needforspeed2d.sh run client --valgrind</code>

Servidor:
<code class="command">./needforspeed2d.sh run server --valgrind</code>

Editor:
<code class="command">./needforspeed2d.sh run editor --valgrind</code>

🎮 Manual del Juego

El juego incluye mapas jugables precargados.
Además, el usuario puede crear mapas personalizados usando el editor interactivo.

Si es la primera vez, se recomienda explorar el editor.

🗺️ 1° Editor de Mapas

Para abrir el editor:

<code class="command">taller_editor</code>

Ciudades disponibles:

San Andreas: avenidas amplias y rectas largas

Vice City: calles angostas y trazados cortos

Liberty City: río central, isla y múltiples puentes

1.1 Colocación de elementos

En la barra superior podés colocar:

Salida

Meta

Checkpoints

El cursor indica si la ubicación es válida.
Los elementos pueden rotarse con R.

Herramientas disponibles:

Borrar

Deshacer (Ctrl + Z)

1.2 Guardado de mapas

Opciones:

Guardar como → crear un nuevo mapa

Abrir mapa jugable → modificar uno existente

Guardar → actualizar el actual

🚀 Iniciar el Juego
1° Servidor

<code class="command">taller_server 8080</code>

2° Cliente

Cada jugador ejecuta:

<code class="command">taller_client localhost 8080</code>

Se mostrarán las opciones:

Crear partida

Unirse a partida

3° Crear Partida

El anfitrión podrá:

Seleccionar nombre

Elegir auto

Elegir mapas jugables

Se genera un código de 4 dígitos para que otros jugadores se unan.

4° Unirse a Partida

El jugador ingresa:

Nombre

Auto

Código de partida

5° Pre-partida / Lobby

Se mostrarán los jugadores y sus autos.
La partida empieza cuando todos estén listos.

🎮 Controles del Juego
Movimiento
Tecla	Acción
W	Avanzar
A	Girar izquierda
S	Retroceder
D	Girar derecha
Misceláneo
Tecla	Acción
M	Silenciar sonidos
N	Subir volumen
B	Bajarlo
Cheats
Tecla	Efecto
P	Forzar derrota
O	Forzar victoria
I	Vida infinita
U	Modo fantasma
🏁 Dinámica del Juego
1. Objetivo

Pasar todos los checkpoints

Cruzar la meta

Evitar pasto/veredas (ralentizan)

2. Sistema de vida

El auto pierde vida al chocar

Si llega a 0:

Se detiene

Explota

Recibe penalización de tiempo

3. Condición de victoria

Gana quien tenga el menor tiempo total al finalizar todos los circuitos.

🛠️ Menú de Mejoras

Entre carreras, los jugadores pueden mejorar su auto.
Cada mejora agrega una penalización de tiempo, por lo que debe usarse estratégicamente.

📊 Sistema de Ranking

Ejemplo:

Carrera	Jugador A	Jugador B
1	10s	11s
2	15s	16s
3	25s	20s

Resultado final:

Jugador A = 50s

Jugador B = 47s → Ganador

🌐 Página Web

Incluye gameplay y tutoriales:

https://joaquinschapira.github.io/taller_TP_pagina_web/

🎥 Video Ejemplo

Video demostrativo del funcionamiento completo:

https://youtu.be/ID62qAriQmw

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