## 3. Matriz de Riesgo
Identificación de posibles problemas durante la implementación.

| Riesgo | Probabilidad | Impacto | Mitigación |
| :--- | :--- | :--- | :--- |
| Incompatibilidad con datos históricos (sin lote). | Alta | Media | Permitir valores nulos solo para registros antiguos o asignar lote genérico. |
| Errores en el formato de fecha al exportar. | Media | Baja | Implementar validaciones de formato ISO en el componente de exportación. |
| Retraso en el cronograma por complejidad en reportes. | Baja | Alta | Revisión de código temprana (Peer Review) y pruebas unitarias. |