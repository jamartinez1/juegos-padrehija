# 👨‍👧 Juegos Papá & Hija

Minijuegos para dos en un mismo celular o tablet. Sin anuncios, sin internet, sin cuentas.

**Para peques (3 años, cooperativos):** Burbujas · Busca el animal · Busca el color · Busca la fruta · Cuenta conmigo · Pintar juntos · Piano · Memoria (nivel Peque).

**Atrapa y gana:** Hipopótamos hambrientos · Atrapa topos · Atrapa estrellas · Pesca.

**Retos papá vs hija:** Tira y afloja · Reflejos · Pong · Duelo de mates · Triqui · Piedra, papel o tijera.

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
