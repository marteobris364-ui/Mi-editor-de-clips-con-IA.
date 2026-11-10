# ClipMaker IA Mobile — MVP 1.0

## Qué está incluido
- UI móvil en español.
- Carga de archivo local.
- Intento de importar URL directa (sujeto a CORS; páginas de YouTube/TikTok no).
- Duración y cantidad configurables; cortes uniformes, desde el inicio o manuales.
- Títulos editables y nombres de archivo.
- Vista previa saltando al inicio del corte.
- Exportación MP4 con FFmpeg WebAssembly (carga CDN).
- Exportar todos los clips, uno por uno.
- Crear archivo SRT con texto pegado y tiempos aproximados.
- Descargar lista de títulos.
- Manifest y service worker para instalación PWA básica.

## Lo que NO está terminado (IA real)
No hay comprensión semántica de audio/video, selección viral garantizada, ASR integrado, eliminación automática de silencios ni extracción de video de plataformas. Esas funciones requieren modelos/API/backend y permisos de las plataformas. La generación de SRT usa tiempos estimados, no sincronía palabra a palabra.

## Cómo abrir
1. Descomprime ZIP.
2. Para probar, abre `index.html` (la importación de módulos/CDN puede estar bloqueada al abrir como file://).
3. Para funcionamiento correcto/PWA, publica la carpeta en HTTPS (GitHub Pages, Netlify o similar).
4. En iPhone Safari, abre la URL HTTPS y usa Compartir → Añadir a pantalla de inicio.

## Limitaciones iPhone
FFmpeg wasm y videos grandes pueden exceder la memoria del navegador. Prueba primero con videos cortos/pequeños. Mantén Safari actualizado y conexión activa.
