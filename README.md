# fondos-emergencia
Actividades Finanzas Personales UNICESMAG

## Archivos

- `index.html` — versión con sincronización Firebase, acceso docente y exportación CSV para Moodle.
- `fondo-emergencia.html` — versión para estudiantes, calificable por estudiante:
  - Al inicio se elige modalidad **individual** o **grupal** (2 a 4 integrantes). En ambas cada estudiante recibe su propia nota.
  - Lección interactiva (simulador con tarro, juego IUN, costo de endeudarse con tarjeta a 12 cuotas y gota a gota, gastos hormiga, reto de 52 semanas) y 4 actividades con gráficos interactivos: tarro y medidor de meses cubiertos, controles deslizantes y proyección semana a semana.
  - Nota por estudiante: Foto financiera 25%, Reto 20%, Crisis 15%, Compromiso 30%, Juego IUN 10%. Cada actividad vale 40% por desarrollo de las respuestas y 60% por sus criterios de aciertos/errores.
  - Al final cada estudiante ve su resumen: nota, situación actual (tarro, meses cubiertos), simulador "¿y si ahorro más?", cobertura ante emergencias, lo que hizo bien, lo que debe mejorar con recomendaciones y un plan de acción con fechas.
  - **Acceso docente** (botón con candado o `fondo-emergencia.html#docente`): panel protegido por contraseña con nota, aciertos y errores por estudiante, errores más frecuentes, resultados del juego IUN, respuestas escritas y exportación CSV para Moodle. Lee los registros de Firebase (`grupos/`); sin conexión muestra solo los datos del dispositivo.
  - La contraseña se guarda solo como hash SHA-256 en la constante `DOC_HASH`. Para cambiarla: `printf '%s' 'NuevaClave' | sha256sum` y reemplazar el valor.
