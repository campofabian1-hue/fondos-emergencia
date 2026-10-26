# fondos-emergencia
Actividades Finanzas Personales UNICESMAG

## Archivos

- `index.html` — versión con sincronización Firebase, acceso docente y exportación CSV para Moodle.
- `fondo-emergencia.html` — versión rediseñada para estudiantes: lección interactiva (simulador de meta, juego "¿es una emergencia?", costo de endeudarse, gastos hormiga), las 4 actividades evaluadas y scorecard. Tema claro/oscuro y autoguardado local.
  - **Acceso docente** (botón con candado o `fondo-emergencia.html#docente`): panel protegido por contraseña con aciertos y errores por grupo y por estudiante, errores más frecuentes, resultados del juego IUN, respuestas escritas y exportación CSV para Moodle. Lee los grupos de Firebase (`grupos/`); sin conexión muestra solo los datos del dispositivo.
  - La contraseña se guarda solo como hash SHA-256 en la constante `DOC_HASH`. Para cambiarla: `printf '%s' 'NuevaClave' | sha256sum` y reemplazar el valor.
