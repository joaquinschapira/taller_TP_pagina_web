<style>
body, p, li, h1, h2, h3, h4, h5, h6 {
  color: #ff00ff !important;
}
</style>
 

# 🔧 Instalación, Compilación y Ejecución

Antes de jugar, es necesario instalar las dependencias y compilar el proyecto. No se necesita conocimiento alguno de C++: todo está automatizado mediante el script needforspeed2d.sh.

 
## 1° Requisitos del Sistema

- Sistema operativo compatible:
  - Ubuntu 24.04 (o distribuciones Linux derivadas)
​

## 2° Otorgar permisos de ejecución

```bash
  chmod +x needforspeed2d.sh
```

## 3° Descargar dependencias:
Este comando instala todas las librerías necesarias (SDL, Qt, cmake, etc.)
```bash
  sudo ./needforspeed2d.sh download
```

## 4° Compilar proyecto
Compilación normal:
```bash
  ./needforspeed2d.sh build
```
Compilación limpia
```bash
  ./needforspeed2d.sh build --clean
  ./needforspeed2d.sh build --c
```

## 5° Ejecutar tests 
```bash
  ./needforspeed2d.sh tests
```

## 6° Ejecutar

- El proyecto incluye tres ejecutables:
  - Cliente
  - Servidor
  - Editor de mapas

Todo se ejecuta desde el instalador.

Cliente:
```bash
  ./needforspeed2d.sh run client
 ```
 Servidor:
 ```bash
  ./needforspeed2d.sh run server
 ```
 Editor:
 ```bash
  ./needforspeed2d.sh run editor
```

## 7° Ejecutar con valgrind (opcional)
Importante:

Cliente y editor usan Valgrind_helpers para supresiones (ver markdown del directorio Valgrind_helpers)

Server no usa supresiones


Cliente:
```bash
  ./needforspeed2d.sh run client --valgrind
 ```
 Servidor:
 ```bash
  ./needforspeed2d.sh run server --valgrind
 ```
 Editor:
 ```bash
  ./needforspeed2d.sh run editor --valgrind
```

## 8° Configuración del software

El archivo de configuración se encuentra en:
```bash
  etc/need4speed/config.yaml
```

Permite modificar: duración de carrera, características de los autos, tiempos de pantallas intermedias y más!

No es necesario modificarlo para jugar.

Recursos utilizados (mapas, texturas, sonidos) se encuentran en:
```bash
  resources/
```

Ya vienen listos al compilar.


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

.container {
  background-color: #1a1a1a;
  padding: 20px;
}

header h1 {
  display: none !important;
}  
</style>

<style>


.container {
  max-width: 900px !important;
  background-color: rgba(0,0,0,0.85);
  padding: 20px;
  border-radius: 8px;
  z-index: 2;
  position: relative;
}


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


@media (min-width: 1200px) {
  body {
    padding-left: 200px;
    padding-right: 200px;
  }
}

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
