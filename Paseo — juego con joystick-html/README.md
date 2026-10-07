# Paseo pixel — juego con joystick

Videojuego en pixel art que se juega en el navegador con un joystick táctil.

## Escenarios

- **Calle**: el restaurante, el hámster Hamy, palomas y un coche que pasa.
- **Restaurante**: gato (tic tac toe) contra la rata malvada; si ganas, el combo es gratis.
- **Boliche**: tira la bola y junta puntos.
- **Café La Lucha**: juego de los vasos con frappés; encuentra la crepa.
- **Cine**: compra palomitas en la dulcería y esquiva los plátanos del mono en la función (con ayuda de Palomín).
- **Cerro de Jicalán**: sube, junta monedas y gana la moto con el memorama.
- **Plaza de Uruapan**: carrera en moto brincando aguacates.

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
