# Informe de Hotfix - Sistema de Matrículas

## 1. Información del Incidente
| Campo | Detalles |
| :--- | :--- |
| **ID CR** | CR-005-SEM4-Minaya-Rafael |
| **Proyecto** | Sistema de Matrículas |
| **Tipo de cambio** | Correctivo (Hotfix) |
| **Prioridad** | Crítica / Inmediata |

## 2. Descripción del Problema
**Incidente:** El sistema duplica pagos en el 1% de las transacciones durante horas pico de alta concurrencia.
**Impacto:** Afectación financiera directa al usuario y descuadre en caja.

## 3. Solución Técnica (Fix)
* **Implementación:** Se añade una "Idempotency Key" en el proceso de pago para ignorar peticiones duplicadas con el mismo ID de sesión.
* **Pruebas:** Simulación de carga con JMeter para verificar que 100 clics simultáneos generen un solo cobro.

## 4. Plan de Rollback
* En caso de error en la validación, revertir al commit anterior y desactivar el trigger de restricción en la base de datos de transacciones.