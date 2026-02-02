# Solicitud de Cambio (CR) - Sistema de Inventario

## 1. Información General
| Campo | Detalles |
| :--- | :--- |
| **ID CR** | CR-004-SEM4-Minaya-Rafael |
| **Proyecto** | Sistema de Inventario |
| **Tipo de cambio** | Funcional (Alcance) |
| **Prioridad** | Alta |
| **Fecha** | 02/02/2026 |

## 2. Descripción del Cambio
**Solicitud:** Agregar campos obligatorios "Lote" y "Fecha de caducidad" en productos perecederos.
**Alcance:** El cambio debe afectar a la base de datos, la interfaz de usuario, los reportes mensuales y los módulos de exportación (CSV/Excel).

## 3. Análisis de Impacto
* **Tiempo:** Estimado de 12 horas de desarrollo.
* **Arquitectura:** Modificación de esquemas en la base de datos.
* **Calidad:** Requiere pruebas de regresión en exportaciones existentes.

## 4. Trazabilidad
* **Requisito:** US-08 Gestión de Perecederos.
* **Código:** Commit vinculado a la rama de mejora funcional.