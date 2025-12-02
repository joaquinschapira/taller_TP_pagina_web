
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

## Instalación y uso básico

### 1. Clonar el repositorio
```bash
git clone https://github.com/lucasPagani2003/taller-de-programacion-tp-grupal-2025c2-grupo-2.git
```

### 2. Otorgar permisos de ejecución al instalador
```bash
chmod +x needforspeed2d.sh
```

### 3. Instalar el proyecto *(una única vez, requiere sudo)*
Este paso debe ejecutarse como root porque instala los binarios y copia assets/config:
```bash
sudo ./needforspeed2d.sh install
```
- ¿Que hace internamente?
    - Instala dependencias esenciales
    - Compila el proyecto
    - Ejecuta los tests del protocolo
    - Instala los ejecutables en el sistema:
        - /usr/bin/taller_client
        - /usr/bin/taller_server
        - /usr/bin/taller_editor
    - Copia recursos del juego a /var/need4speed
    - Copia la configuración a /etc/need4speed
    - En cambio, los mapas jugables se guardan en ~/.local/share/need4speed/mapas_jugables

No es necesario modificar nada para jugar, pero es posible personalizar desde config

### 4. Ejecutar los programas
Editor de mapas:
```bash
taller_editor
```

Servidor:
```bash
taller_server 8080
```

Cliente:
```bash
taller_client localhost 8080
```

---

## Más información
Para ver todos los comandos disponibles y detalles completos de compilación/uso, consultá el [manual de usuario](./Manual_de_Usuario.pdf).

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