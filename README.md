# weather-frontend-m4
Proyecto portafolio / Módulo IV / Bootcamp Frontend TD

Visita el proyecto en: https://ramirezjm.github.io/weather-frontend-m4/

ClimApp es una aplicación que entrega pronósticos meteorólogicos precisos y personalizados. Ofrecemos una muestra de nuestro trabajo con una selección de distintas ciudades del mundo.

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
![Static Badge](https://img.shields.io/badge/HTML5-%23f06529)
![Static Badge](https://img.shields.io/badge/CSS3-%232965f1)
![Static Badge](https://img.shields.io/badge/Javascript-%23f0db4f)
![Static Badge](https://img.shields.io/badge/Bootstrap-8A2BE2)
![Static Badge](https://img.shields.io/badge/Sass-CC6699)

<div><img src='./assets/images/screenshot1.jpg' width=600></div>
<div><img src='./assets/images/screenshot2.jpg' width=600></div>
<div><img src='./assets/images/screenshot4.jpg' width=600></div>

### Modelado de datos

- La aplicación trabaja con un array de objetos que representa distintas ciudades.
- Cada ciudad contiene información general del clima actual (temperatura, estado, humedad y viento) y un array adicional con el pronóstico de la semana.

Este modelo permite reutilizar los datos para generar de forma dinámica las tarjetas de ciudades y el contenido del modal de detalles.

### Estadísticas

En esta versión, la aplicación calcula estadísticas a partir del pronóstico semanal de cada ciudad:
- Temperatura máxima de la semana
- Temperatura mínima de la semana
- Temperatura promedio semanal
- Cantidad de días por tipo de clima (soleado, nublado, lluvioso, etc.)
- Un mensaje resumen que describe el clima predominante de la semana (por ejemplo, “Semana mayormente despejada”)

Los cálculos se realizan mediante ciclos y condicionales en JavaScript, y los resultados se renderizan dinámicamente en el modal de detalles.

#### 1. Clonar el repositorio

  ```bash
   git clone https://github.com/RamirezJM/weather-frontend-m4.git
   cd weather-frontend-m4
```

#### 2. Instalar dependencias

```bash
npm install
```

#### 3. Compilar Sass

 ```bash
npm run watch:css
```

#### 4. Ejecutar el el proceso de build

```bash
npm run build:css
```

--> Build incluye __purgecss__, que permite eliminar todas las clases no usadas una vez desplegado el proyecto, reduciendo el peso del archivo final compilado (~250kb -> ~50kb), y borrando alrededor de 10.000 líneas de código no utilizado. Se incluye una _safelist_ para resguardar las clases usadas y evitar que sean borradas.

