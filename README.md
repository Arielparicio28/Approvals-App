# Aprobaciones CILSA

## Descripción

Se ha desarrollado una aplicación de aprobaciones en **Microsoft Power Apps** para el cliente **CILSA**, con el objetivo de gestionar y automatizar los procesos de aprobación dentro de la organización.

La solución está integrada con el ecosistema de **Microsoft Power Platform** y utiliza **Microsoft Dataverse** como repositorio de datos para la aplicación.

## Arquitectura de Integración

La aplicación obtiene información procedente de **Microsoft Dynamics 365 Finance & Operations (F&O)** mediante la tecnología **Dual-write**.

### Flujo de Datos

1. Los datos maestros y transaccionales se gestionan en **Dynamics 365 Finance & Operations**.
2. **Dual-write** sincroniza automáticamente las entidades configuradas entre Finance & Operations y Dataverse.
3. La aplicación de **Power Apps** consume los datos almacenados en **Dataverse**.
4. Los usuarios realizan las aprobaciones a través de la interfaz de Power Apps.
5. La información de aprobación queda registrada y disponible para su posterior explotación y seguimiento.

## Tecnologías Utilizadas

* Microsoft Power Apps
* Microsoft Dataverse
* Microsoft Dynamics 365 Finance & Operations
* Dual-write
* Power Platform

## Beneficios de la Solución

* Centralización de los procesos de aprobación.
* Integración nativa con Dynamics 365 Finance & Operations.
* Sincronización automática de datos mediante Dual-write.
* Reducción de tareas manuales y errores de captura.
* Mayor trazabilidad y control de las aprobaciones.
* Experiencia de usuario optimizada mediante Power Apps.

## Dependencias

* Entorno de Microsoft Power Platform configurado.
* Instancia de Microsoft Dynamics 365 Finance & Operations.
* Configuración activa de Dual-write entre F&O y Dataverse.
* Permisos adecuados para los usuarios finales y administradores.

## Consideraciones

* Las tablas de Dataverse utilizadas por la aplicación deben estar correctamente sincronizadas mediante Dual-write.
* Cualquier modificación en las entidades sincronizadas debe ser evaluada para garantizar la compatibilidad con la aplicación.
* Se recomienda monitorizar periódicamente el estado de sincronización de Dual-write para asegurar la integridad de los datos.

## Cliente

**CILSA**


Desarrollo realizado en Microsoft Power Apps con integración a Dynamics 365 Finance & Operations mediante Dual-write.
