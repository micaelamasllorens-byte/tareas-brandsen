# Tareas Kiosco Brandsen

Checklist de tareas por turno del Kiosco Brandsen (Brandsen 119, Quilmes).

- Cada empleado elige su turno, tilda las tareas (queda la hora de cada tic) y al cerrar elige el motivo de lo que no se hizo.
- Al cerrar el turno se arma un resumen listo para pegar en el grupo de WhatsApp.
- Selector de días: se puede ver la lista de cualquier día y cómo quedó ese turno la última vez.
- "Administrar tareas" (con código) permite agregar, eliminar y reordenar tareas, ver el historial y cambiar el código.

## Cómo está armado

- `index.html`: toda la app en un solo archivo, publicada con GitHub Pages.
- Los datos se guardan en un proyecto de Supabase propio (`tareas-brandsen`), separado de la web del kiosco.
  - `turnos`: turnos de la semana con sus bloques y tareas. Solo se modifican con el código de administración.
  - `registros`: lo que se tildó en cada turno, por fecha.
  - `config_admin`: el código de administración, guardado cifrado y no accesible desde la página.
