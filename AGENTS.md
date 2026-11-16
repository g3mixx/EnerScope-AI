# Guía para agentes de desarrollo — EnerScope AI

## Orientación rápida
- API/negocio: `backend/app/`.
- Almacenamiento y migraciones: `backend/app/database.py` y `backend/migrations/`.
- Extracción de recibos: `backend/app/extraction.py`.
- Finanzas y métricas: `backend/app/analytics.py`, `backend/app/financial_analytics.py`, `backend/app/numeric.py`.
- Análisis opcional por IA: `backend/app/receipt_analysis.py`, `backend/app/agent.py`.
- Interfaz React: `frontend/src/`.
- Informes: `backend/app/reporting.py`.
- Instalación: `INSTALAR.bat`, `INICIAR.bat`, `scripts/`.

## Economía de contexto y tokens
1. Investiga primero nombres y referencias con búsquedas dirigidas (`rg`, símbolos o Graphify si está instalado).
2. Lee solo las funciones y archivos afectados; evita volcar el proyecto completo en cada turno.
3. Reutiliza la documentación de decisiones y contratos existentes.
4. Realiza commits acotados y registra qué cambió y qué pruebas pasaron.
5. No reconstruyas el grafo en cada pregunta: actualízalo solo tras cambios relevantes.
6. Mantén los cálculos contables en Python; no delegues aritmética crítica a LLM.
7. Para IA por recibo, usa datos confirmados y estructurados, fingerprint/versionado y resultados persistentes. No llames a un modelo durante GET o render del dashboard.
8. No envíes texto completo de todos los PDF si bastan los campos confirmados, los totales calculados y evidencias puntuales.

## Restricciones
- No usar recibos, claves, RPU ni bases reales para pruebas; únicamente sintéticos.
- No precargar empresas, consumos, facturas ni análisis de ejemplo en producción.
- No duplicar cargos o bonificaciones al calcular subtotales.
- No modificar migraciones históricas sin una razón fundada y compatibilidad revisada.
- No exponer credenciales en código, README, CI ni logs.
- Si una acción requiere acceso a producción o datos privados, solicita autorización explícita.

## Verificaciones
Ejecuta las pruebas disponibles, compilación frontend y verificación de archivos. Informa los bloqueos de entorno; nunca afirmes que una comprobación pasó si no se ejecutó.