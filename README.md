# Control de gastos 2026 (v1.3)

App web instalable (PWA) para registrar ingresos y gastos, controlar el presupuesto por categoría y ver el resumen anual. Funciona sin internet una vez abierta. No usa librerías externas.

## Archivos (todos en la raíz del repositorio)
`index.html` · `manifest.json` · `sw.js` · `icon-192.png` · `icon-512.png` · `icon-maskable-512.png` · `README.md`

## Funciones
- Registro de ingresos y gastos con fecha, categoría, descripción y monto.
- Panel del mes (ingresos, gastos, saldo, saldo acumulado) y resumen anual con gráfica.
- Presupuesto por categoría con estados (dentro, cerca del límite, excedido) y alertas.
- Exportar a Excel (.xlsx) con hojas Resumen, Ingresos y Gastos (fórmulas incluidas).
- Seguridad opcional: PIN de 4 o 6 dígitos, huella/biometría y código de recuperación.
- Modo claro/oscuro automático.

## Publicar en GitHub Pages
1. Crea un repositorio y sube los 7 archivos a la raíz ("uploading an existing file").
2. Settings > Pages > rama `main`, carpeta `/ (root)`.
3. Abre el link HTTPS en el celular.

## Instalar como aplicación
- Android (Chrome): menú ⋮ > "Instalar aplicación".
- iPhone (Safari): Compartir > "Agregar a pantalla de inicio".
- Computador (Chrome/Edge): ícono de instalar en la barra de direcciones.

## Actualizar
Al cambiar `index.html`, cambia la versión en `sw.js` (`const V = 'control-gastos-v1.3.1'`) para que los dispositivos reciban la actualización.

## Datos y privacidad
Todo se guarda solo en el navegador del dispositivo (localStorage). El PIN bloquea la pantalla pero no cifra los datos. Los valores de presupuesto por categoría son de ejemplo y se editan en el código (`PRES`).
