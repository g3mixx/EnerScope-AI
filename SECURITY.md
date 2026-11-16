# Seguridad

## Reportar una vulnerabilidad
No publiques detalles de explotación, credenciales ni información de clientes en issues públicos. Contacta al mantenedor [@g3mixx](https://github.com/g3mixx) por un canal privado para coordinar la divulgación.

## Modelo de amenazas
EnerScope procesa archivos PDF aportados por usuarios y conserva información de facturación en SQLite local. No debe exponerse directamente como servicio público sin autenticación, controles adicionales y revisión independiente.

- No ejecutes archivos PDF como código.
- Mantén dependencias actualizadas; verifica las entradas y el tamaño de archivos.
- Usa bases de pruebas aisladas; jamás bases de clientes para CI.
- La IA es opcional y puede transmitir el contenido seleccionado de recibos al proveedor conectado.
- No subas archivos `.env`, directorios `data/`, `*.db`, recibos ni tokens a GitHub.
- Antes de compartir registros, elimina identificadores, rutas personales y contenido privado.

## Alcance
La publicación del código no implica una certificación de seguridad o precisión tarifaria. Las decisiones económicas deben contrastarse con los documentos originales y un profesional competente.