# Informe de Configuración de Seguridad - API REST

## 1. Información del Cambio
| Campo | Detalles |
| :--- | :--- |
| **ID CR** | CR-006-SEM4-Minaya-Rafael |
| **Proyecto** | API REST |
| **Tipo de cambio** | Configuración / Seguridad |
| **Prioridad** | Media |

## 2. Descripción de la Mejora
**Solicitud:** Reducir el tiempo de expiración (TTL) de los tokens JWT de 24 horas a 1 hora y habilitar la rotación automática de llaves criptográficas.
**Objetivo:** Minimizar la ventana de exposición en caso de robo de tokens y cumplir con los estándares de seguridad OWASP.

## 3. Impacto y Pruebas
* **Impacto en Clientes:** Se requiere la implementación de "Refresh Tokens" para evitar que el usuario tenga que loguearse manualmente cada hora.
* **Prueba de Integración:** Verificación de rechazo de tokens antiguos tras la rotación de la llave maestra.

## 4. Trazabilidad
* **Origen:** Auditoría de Seguridad interna / Hardening de Infraestructura.
* **Evidencia:** Logs de validación de expiración en entorno de Staging.