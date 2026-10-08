# Paseo pixel — juego con joystick

Videojuego en pixel art que se juega en el navegador con un joystick táctil.

## Escenarios

- **Mapa de Uruapan** (pantalla de inicio): toca un lugar para ir; el botón MAPA te regresa.

- **Calle**: el restaurante, el hámster Hamy, palomas y un coche que pasa.
- **Restaurante**: gato (tic tac toe) contra la rata malvada; si ganas, el combo es gratis.
- **Boliche**: tira la bola y junta puntos.
- **Café La Lucha**: juego de los vasos con frappés; encuentra la crepa.
- **Gimnasio** (bajando desde el café): press de banca manteniendo presionado; al completar la serie se desbloquea Mandarina, una gata naranja que te acompaña.
- **Parque La Pinera**: columpio (impulsa en el momento justo) y resbaladilla.
- **Cine**: compra palomitas en la dulcería y esquiva los plátanos del mono en la función (con ayuda de Palomín).
- **Cerro de Jicalán**: sube, junta monedas y gana la moto con el memorama.
- **Plaza de Uruapan**: carrera en moto brincando aguacates.

## Monedas y terreno

Cada minijuego da monedas: memorama 100, columpio 30, gato 30 (empate 5), función 25, vasos 20, gimnasio 15, boliche 2–5, resbaladilla 3 y la carrera 1 por cada 20 m. Con 300 se canjea la moto y con 600 se compra un terreno desde el mapa.

## Cómo jugarlo en tu computadora

Los navegadores bloquean los scripts si abres el archivo con doble clic, así que hay que servir la carpeta:

- **VS Code**: instala la extensión *Live Server*, da clic derecho en `index.html` → *Open with Live Server*.
- **Terminal**: `python -m http.server` dentro de esta carpeta y abre <http://localhost:8000>.

## Publicarlo en internet (GitHub Pages)

En el repositorio de GitHub: *Settings* → *Pages* → *Source: Deploy from a branch* → rama `main`, carpeta `/ (root)` → *Save*.
En un par de minutos queda en `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

## Archivos

- `Main.dc.html` — el juego completo: escenas (marcado) y lógica (la clase `Component` al final).
- `index.html` — página de entrada que abre el juego.
- `assets/` — imágenes pixeladas (fondos, personajes, objetos).
- `support.js`, `vendor/` — el motor que dibuja el juego en el navegador; no hace falta editarlos.

## Desplegar en Railway

El proyecto trae `package.json` y `server.js` (un servidor de Node sin dependencias), así que Railway lo detecta como app de Node y corre `npm start`.

1. Sube los cambios a GitHub.
2. En Railway: *New Project* → *Deploy from GitHub repo* → elige el repositorio.
3. Si los archivos del juego están dentro de una subcarpeta del repo, en *Settings* → *Root Directory* pon esa carpeta.
4. En *Settings* → *Networking* da clic en *Generate Domain* para obtener el link público.
