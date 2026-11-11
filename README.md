# 👨‍👧 Juegos Papá & Hija

Minijuegos para dos en un mismo celular o tablet. Sin anuncios, sin internet, sin cuentas.

**Aprender juntos (nadie pierde):** Busca el animal · Busca el color · Formas · Sombras · Grande y pequeño · ¿Qué come? · ¿De qué color es? · Busca la fruta · Cuenta conmigo · Alimenta al dino · Vocales · Emociones · Camino.

**Jugar juntos:** Burbujas · Globos de colores · Pintar juntos · Piano.

**De suerte (cualquiera gana):** Carrera de dados · Escondite · Memoria.

**Atrapa y gana:** Hipopótamos hambrientos · Atrapa topos · Atrapa estrellas · Pesca · Tira y afloja.

**Para cuando crezca:** Reflejos · Pong · Duelo de mates · Triqui · Piedra, papel o tijera.

Nivel "Peque": 3 opciones por pregunta, contar hasta 3 y memoria de 8 cartas.
Para salir de un juego se mantiene presionada la ✕.

El jugador de abajo es el 1 (azul) y el de arriba el 2 (rosa, pantalla girada hacia él).
El marcador y los nombres se guardan en el dispositivo.

## Probar en el computador
```bash
cd juegos-padrehija
python3 -m http.server 8000
```
Abre http://localhost:8000. Desde el celular (misma wifi): `http://<IP-de-tu-Mac>:8000`.

## Instalarlo en el celular
Súbelo gratis a Netlify / GitHub Pages / Cloudflare Pages (solo es una carpeta estática),
ábrelo en el celular y usa "Añadir a pantalla de inicio". Luego funciona sin conexión.

## Agregar un juego
En `index.html`: escribe una función `miJuego(G)` (usa `G.split()`, `G.after()`, `G.countdown()`,
`G.end(ganador)`) y añádela al arreglo `GAMES`.
