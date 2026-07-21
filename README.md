# ALE.INK — Sitio web + Panel del artista

Sitio web para el estudio de tatuajes de **Alejandro Briceño** (Viña del Mar).

## Estructura

- `index.html` — Landing pública. Portafolio, flash shop y cotizador.
- `panel-artista.html` — Panel privado del artista (acceso con PIN).
- `assets/` — Imágenes y videos del sitio.
- `netlify.toml` — Configuración de despliegue.

## Cómo funciona

1. Un cliente llena el cotizador en la landing (estilo, zona, tamaño, contacto).
2. Se abre WhatsApp con el mensaje pre-armado hacia el artista (aviso inmediato).
3. La cotización queda guardada y aparece en el Panel del artista, sincronizada
   entre todos sus dispositivos.
4. Desde el panel, el artista revisa, aprueba, pone precio, agenda y ve estadísticas.

## Backend

Los datos se guardan en Google Sheets vía Google Apps Script (gratis, sin servidor
propio). El código del backend está en `../backend-google-sheets/Code.gs`.
Pega la URL de tu implementación en la constante `ALEINK_API_URL` de ambos HTML.

## Panel privado

- URL: `/panel` (o `/panel-artista.html`)
- PIN por defecto: `1234` — cambiarlo en Ajustes tras el primer ingreso.

---
Desarrollado por Clickeao.
