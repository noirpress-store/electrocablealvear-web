# Electro Cable Alvear — Landing

Sitio hecho con Vite + React. Todo el contenido (logos, marcas, mapa) está
incrustado, no requiere archivos externos. Los datos editables del negocio
están en el bloque `CONFIG` al inicio de `src/App.jsx`.

## Desarrollo local
```bash
npm install
npm run dev        # http://localhost:5173
npm run build      # genera /dist para producción
```

## Deploy con GitHub + Vercel

### 1) Subir a GitHub
```bash
cd electrocablealvear-web
git remote add origin https://github.com/noirpress-store/electrocablealvear-web.git
git branch -M main
git push -u origin main
```
(Creá antes el repo vacío `electrocablealvear-web` en la cuenta noirpress-store: https://github.com/new — sin README.)

### 2) Importar en Vercel
1. Entrá a https://vercel.com/new
2. Importá el repo `electrocablealvear-web`.
3. Vercel detecta **Vite** automáticamente (Build: `npm run build`, Output: `dist`).
4. Deploy. Queda publicado en `https://electrocablealvear-web.vercel.app`
   (podés renombrar el proyecto en Vercel para tener `electrocablealvear.vercel.app`).

Cada `git push` a `main` redeploya solo.

## Editar datos del negocio
Abrí `src/App.jsx` → bloque `CONFIG` (WhatsApp, dirección, horarios, mapa, marcas).
