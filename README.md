# Mi Equipo — Planificador semanal

App web progresiva (PWA) para gestionar horarios, asistencia y notas de tu equipo de trabajo. Instalable en iPhone como app nativa.

## Funciones

- Registro de asistencia diaria por trabajador (Presente, Ausente, Tarde, No corresponde)
- Control de horarios de entrada y salida
- Notas por día y por trabajador
- Resumen semanal con gráficos por persona y por equipo
- Autoguardado automático
- Funciona sin internet (modo offline)
- Instalable en iPhone como app nativa

## Cómo instalar en iPhone

1. Abre Safari y ve a: `https://TU_USUARIO.github.io/mi-equipo`
2. Toca el botón compartir (cuadro con flecha hacia arriba)
3. Selecciona **"Añadir a pantalla de inicio"**
4. Toca **Añadir** — la app aparecerá como ícono en tu pantalla

## Cómo subir a GitHub Pages

1. Crea un repositorio nuevo en github.com llamado `mi-equipo`
2. Sube todos estos archivos al repositorio
3. Ve a **Settings → Pages**
4. En "Source" selecciona **Deploy from a branch → main → / (root)**
5. Guarda — en unos minutos estará en: `https://TU_USUARIO.github.io/mi-equipo`

## Archivos del proyecto

```
mi-equipo/
├── index.html       ← App principal
├── manifest.json    ← Configuración PWA
├── sw.js            ← Service worker (offline)
├── icons/
│   ├── icon-192.png
│   └── icon-512.png
└── README.md
```

## Personalizar trabajadores

Los nombres de ejemplo se pueden editar directamente en `index.html`, buscando esta línea:

```js
let members = JSON.parse(localStorage.getItem('mieq_members') || '["Ana García","Carlos López",...]');
```

Cambia los nombres por los de tu equipo real.
