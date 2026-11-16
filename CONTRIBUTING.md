# Contribuir a EnerScope AI

¡Gracias por mejorar el proyecto! Prioriza correcciones reproducibles y cambios pequeños.

## Preparación
- Python 3.12, Node.js y npm.
- Instala las dependencias de `requirements.txt` en un entorno virtual.
- En `frontend/`, ejecuta `npm ci`, `npm run build` y las comprobaciones disponibles.
- Utiliza solo PDF y bases SQLite **sintéticos** para las pruebas.

## Flujo de colaboración
1. Abre un issue explicando problema, versión y pasos de reproducción.
2. Crea una rama específica (por ejemplo `fix/receipt-sorting`).
3. Mantén independientes los commits y evita refactorizaciones ajenas al objetivo.
4. Agrega pruebas de regresión, especialmente para importes, RPU, fechas y ámbitos por empresa.
5. Envía un pull request con los resultados comprobados y limitaciones.

## Seguridad
Nunca adjuntes recibos de clientes, RPU reales, capturas con datos privados, SQLite, claves, cookies ni tokens. Los ejemplos deben ser inventados.

## Política de IA
Se aceptan contribuciones asistidas por IA, pero los cambios deben ser revisados, atribuidos con honestidad y probados. No declares pruebas no ejecutadas.

## Licencia
El repositorio todavía no ha adoptado una licencia open source; solicita autorización del propietario antes de redistribuir el código.