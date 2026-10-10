# Control de Frentes — app instalable

Esta carpeta es un "marco" para GitHub Pages: muestra la web app de Apps Script a pantalla completa
y permite instalarla (escritorio o celular) con su propio icono. No guarda datos: todo vive en tu Google Sheet.

## Configurar
1. En `index.html`, reemplaza `APP_URL` por tu URL de Apps Script que termina en `/exec`.
2. Sube todos los archivos de esta carpeta a la raíz de un repositorio (por ejemplo `control-de-frentes`).
3. En GitHub: Settings › Pages › Source: *Deploy from a branch* › rama `main` › carpeta `/ (root)`.
4. Abre `https://TU-USUARIO.github.io/control-de-frentes/` e instala:
   - Chrome/Edge (PC): icono de instalar en la barra de direcciones.
   - Android (Chrome): menú ⋮ › Instalar app / Agregar a pantalla principal.
   - iPhone (Safari): Compartir › Agregar a pantalla de inicio.

## Notas
- La URL del repositorio es pública, pero la app solo abre con tu cuenta (implementación "Solo yo").
- Si el marco no carga o pide iniciar sesión, usa el enlace "Abre la app directamente" y verifica que
  solo tengas tu Gmail abierto en ese navegador. En iPhone, Safari puede bloquear la sesión dentro del marco.
- Si cambias `index.html` y no ves el cambio, cierra y vuelve a abrir la app (el service worker se actualiza solo).
