# Invitación de Casamiento

Invitación web con contador en tiempo real (días, horas, minutos y segundos) hasta la fecha del casamiento.

## Cómo verla

Abrí `index.html` con doble clic, o arrastralo a cualquier navegador (Chrome, Firefox, etc). No necesita instalación ni servidor.

## Cómo personalizarla

Abrí `index.html` con un editor de texto (Notepad, VS Code, Sublime, etc.) y buscá estos bloques:

1. **Nombres de los novios**
   ```html
   <h1 class="names">Julieta<span class="amp">&amp;</span>Tomás</h1>
   ```

2. **Fecha y lugar (texto que se muestra)**
   ```html
   <div class="date-block">Sábado 12 de Diciembre de 2026 · 19:00 hs</div>
   <div class="place-block">Quinta El Ombú — La Plata, Buenos Aires</div>
   ```

3. **Fecha real del contador** (al final del archivo, dentro del `<script>`)
   ```js
   const weddingDate = new Date('2026-12-12T19:00:00');
   ```
   Formato: `'AAAA-MM-DDTHH:MM:SS'`, en hora local.

4. **Fecha límite de confirmación (RSVP)**
   ```html
   <div class="rsvp">Confirmar asistencia antes del <b>1 de Noviembre</b></div>
   ```

5. **Colores** (arriba del todo, en `:root`) si querés cambiar la paleta.

## Cómo compartirla

- Subila a un hosting gratuito como [Netlify Drop](https://app.netlify.com/drop) o [GitHub Pages](https://pages.github.com/) arrastrando la carpeta, y vas a tener un link para mandar por WhatsApp.
- O simplemente enviá el archivo `index.html` y que cada invitado lo abra en su navegador.

## Estructura

```
invitacion-casamiento/
├── index.html   ← todo el código (HTML + CSS + JS) en un solo archivo
└── README.md    ← este archivo
```
