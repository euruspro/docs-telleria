---
description: >-
  El Módulo DIN dispone del listado de Despachos de Importación correspondientes
  a Declaraciones de Ingreso tramitadas en la Agencia.
---

# Módulo DIN

## Cómo se ordenan las DIN&#x20;

{% hint style="danger" %}
**Priorización de los despachos**

Por defecto, los despachos están ordenados por prioridad, del más al menos **Urgente**.
{% endhint %}

Los despachos son desplegados según su priorización de atención, considerando el siguiente orden:

1. <mark style="color:orange;">**Naranja**</mark>**,** los clasificados como urgentes.
2. <mark style="color:blue;">**Azul**</mark>**,** los que no poseen Fecha Manifiesto, Fecha ETA o Vía de Transporte.
3. <mark style="color:red;">**Rojo**</mark>**,** los vencidos por Fecha Manifiesto, Fecha ETA o por superar el plazo establecido para el estado DIN.
4. **Amarillo**, los vencidos por Fecha Manifiesto, Fecha ETA o los que aún no vencen por permanencia en estado DIN, pero han superado la mitad del plazo establecido.

### Plazos de ejecución para una DIN

Cada despacho DIN obtendrá un un plazo diferente de ejecución según Vía de Transporte o caso especial:

{% hint style="info" %}
Los plazos establecidos están definidos por **horas** **hábiles.**&#x20;
{% endhint %}

#### Pendientes en Ejecutivos

| Vía de Transporte          | Tiempo  |
| -------------------------- | ------- |
| **Operaciones aéreas**     | 8 h     |
| **Operaciones marítimas**  | 16 h    |
| **Operaciones terrestres** | 16 h    |

Existen algunos casos especiales, los cuales cuentan con los siguientes plazos:

| Caso                    | Tiempo |
| ----------------------- | ------ |
| **Operaciones con CDA** | 8 h    |

**Pendientes en Pedidores**

| Vía de Transporte          | Tiempo  |
| -------------------------- | ------- |
| **Operaciones aéreas**     | 5 h     |
| **Operaciones marítimas**  | 16 h    |
| **Operaciones terrestres** | 5 h     |

También se consideran plazos especiales en los que se añaden horas al plazo calculado inicialmente:&#x20;

| Caso                         | Tiempo |
| ---------------------------- | ------ |
| **DIN con 6 a 25 ítems**     | + 1 h  |
| **DIN con 25 a 100 ítems**   | + 4 h  |
| **DIN con más de 100 ítems** | + 8 h  |

{% hint style="warning" %}
Los plazos establecidos está definidos por **horas hábiles,** considerando un horario de Lunes a Viernes desde las 8 hasta las 18 horas.
{% endhint %}

## Qué es Estado DIN <a href="#estado-din" id="estado-din"></a>

Cada despacho se encuentra en una etapa diferente del flujo operacional siendo categorizado por uno de los siguientes Estados DIN:

| Estado DIN                                                                        | Situación del Despacho                                                                                                     |
| --------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| <mark style="color:blue;background-color:blue;">**Etapa de Ejecutivos**</mark>    |                                                                                                                            |
|   **Despacho Aperturado**                                                         | Estado inicial, cuando el despacho es creado y no tiene documentos cargados.                                               |
|   **D**o**cumentos en Revisión**                                                  | Despacho en revisión de documentos requeridos.                                                                             |
|   **Documentos Incompletos**                                                      | El despacho cuenta con documentos pero aun le faltan documentos requeridos.                                                |
|   **Documentos Completos**                                                        | Despacho cuenta con todos los documentos requeridos cargados, revisados y validados.                                       |
| <mark style="color:orange;background-color:orange;">**Etapa de Pedidores**</mark> |                                                                                                                            |
|   **Despacho para Adelantar**                                                     | Despacho tiene documentos incompletos, pero fue entregado a Pedidor para que adelante proceso y deje listo para presentar. |
|   **Pendiente Presentación DIN**                                                  | Despacho con documentación completa y listo para presentación DIN.                                                         |
|   **Pendiente Aceptación DIN**                                                    | Despacho con DIN Presentada.                                                                                               |
|   **Rechazado Sistema Aduana**                                                    | Despacho con DIN Rechazada.                                                                                                |
| <mark style="color:purple;background-color:purple;">Etapas de Finalización</mark> |                                                                                                                            |
|   **Pendiente Pago Impuestos**                                                    | Despacho disponible para pago GCP desde Tesorería.                                                                         |
|   **Pendiente Retiro**                                                            | Despacho disponible para retirar mercancía desde Sucursal.                                                                 |
|   **Pendiente UyD SEREMI**                                                        | Despacho disponible para ingresar N° y Fecha Resolución.                                                                   |
| <mark style="color:green;background-color:green;">Etapas de Cierre</mark>         |                                                                                                                            |
|   **Finalizada (Retiro)**                                                         | Operación finalizada con retiro de carga.                                                                                  |
|   **Finalizada (Pago Impuestos)**                                                 | Operación finalizada con pago GCP.                                                                                         |
|   **Finalizada (UyD SEREMI)**                                                     | Operación finalizada con  CDA SEREMI.                                                                                      |
|   **Finalizada (UyD ISP Importador)**                                             | Operación finalizada con CDA ISP.                                                                                          |
|   **DIN Anulada**                                                                 | Operación anulada.                                                                                                         |

### Definición de Fechas

Las siguientes fechas con asignadas de manera automática por el sistema, tenga presente las condiciones para que cada fecha pueda operar según lo esperado.

| Nombre Fecha | Requisitos                                   | Descripción                                                              |
| ------------ | -------------------------------------------- | ------------------------------------------------------------------------ |
| Fecha Arribo | <p>Vía de transporte.<br>Núm. Manifiesto</p> | Obtiene la fecha real de arribo desde Manifestación Naviera de aduana.cl |
|              |                                              |                                                                          |
|              |                                              |                                                                          |
|              |                                              |                                                                          |

## Vistas

Existen vistas definidas de acuerdo al perfil del usuario, cuya funcionalidad es agrupar y categorizar las operaciones para su gestión. A continuación, se definen las siguientes vistas:

{% hint style="info" %}
Para las siguientes definiciones **las sucursales se consideran como grupos.** Las únicas vistas que no consideran las sucursales son "Mis DIN Pendientes" y "Pendientes del Grupo".
{% endhint %}

| Vista                              | Definición                                                                                                      |
| ---------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| **Mis DIN Pendientes**             | Despachos asignados al usuario.                                                                                 |
| **Pendientes del Grupo**           | Despachos a cargo del grupo del usuario.                                                                        |
| **Pendientes En Ejecutivos**       | Despachos del grupo con estado Documentos en Revisión o Documentos Incompletos.                                 |
| **Pendientes En Pedidores**        | Despachos del grupo con estado Pendiente Presentación DIN, Pendiente Aceptación DIN o Rechazado Sistema Aduana. |
| **Pendientes Inscripción**         | Despachos del grupo con estado Por Corregir Inscripción, Por Inscribir Directo, Por Inscribir Pronto Directo    |
| **Pendientes Garantización**       | Despachos del grupo con estado Por Garantizar, Por Corregir Garantía                                            |
| **Pendientes Aforo**               | Despachos del grupo con estado Aforo Pendiente                                                                  |
| **Pendientes de Retiro**           | Despachos del grupo con estado Pendiente Retiro.                                                                |
| **Pendientes Pago Impuestos**      | Despachos del grupo con estado Pendiente Pago Impuestos (GCP).                                                  |
| **Pendientes Pago Imptos/Agencia** | Despachos del grupo con estado Pendiente Pago Impuestos (GCP)por parte de la Agencia.                           |
| **Pendientes Pago Imptos/Cliente** | Despachos del grupo con estado Pendiente Pago Impuestos (GCP) por parte del Cliente                             |
| **Pendientes UyD SEREMI**          | Despachos del grupo con estado Pendiente UyD SEREMI.                                                            |
| **DIN en Curso**                   | Despachos del grupo con estado diferente a "Finalizada" y "DIN Anulada"                                         |
| **DIN Finalizadas**                | Despachos del grupo con estados "Finalizada".                                                                   |
| **DIN Anuladas**                   | Despachos del grupo con estado DIN Anulada.                                                                     |

### Gestión Documental

Dentro del módulo DIN se encuentra el módulo Documentos donde se realiza toda la gestión documental del despacho, cuyo estado documental resulta de las combinaciones de los estados de los registros, según lo definido por la agencia.

A continuación se muestra una tabla con los estados que se le van asignando a los registros

| Estado Documento    | Descripción                                                                                               |
| ------------------- | --------------------------------------------------------------------------------------------------------- |
| Por Revisar         | Aplica a los registros que se les ha cargado un documento, pero no ha sido validado aún por el ejecutivo. |
| Conforme            | Aplica a los registros que se encuentran validados por el ejecutivo y están aprobados.                    |
| No conforme         | Aplica para los registros que tras ser revisados por el ejecutivo, se encuentran rechazados.              |
| Doc. Complementario | No influye en el estado documental                                                                        |
| Carpeta Electrónica | Todo registro que es creado desde carpeta electrónica.                                                    |

