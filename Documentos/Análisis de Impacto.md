## 2. Análisis de Impacto
Evaluación de las áreas afectadas por la implementación de los campos de Lote y Caducidad.

| Área | Impacto | Evidencia / Nota |
| :--- | :--- | :--- |
| **Alcance** | Cambia | Se agregan nuevos campos obligatorios a los esquemas de productos. |
| **Tiempo** | +12 horas | Estimación para desarrollo de backend, frontend y actualización de reportes. |
| **Costo** | Neutro | Se cubre con los recursos actuales del equipo de desarrollo. |
| **Calidad** | Riesgos a QA | Requiere pruebas de regresión en el módulo de exportación. |
| **Arquitectura** | Afectados | Modificación en la tabla de la base de datos y esquemas de la API. |
| **Seguridad** | No afecta | No se modifican controles de acceso ni autenticación. |
| **Operación** | Despliegue | Requiere script de migración de base de datos para producción. |