---
description: >-
  El Módulo DUS dispone del listado de Despachos de Exportación correspondientes
  a Declaraciones Únicos de Salida tramitadas en la Agencia.
---

# Módulo DUS

## Qué es Estado DUS

Los despachos se encuentran categorizados de acuerdo al estado DUS en que se encuentren. A continuación se listan los estados.

<table><thead><tr><th>Estado DUS</th><th>Descripción</th><th data-hidden></th></tr></thead><tbody><tr><td>Pend. Presentación DUS AT</td><td>El despacho se encuentra en proceso de legalización</td><td></td></tr><tr><td>Pend. Aceptación DUS AT</td><td>El despacho se encuentra con DUS AT presentado</td><td></td></tr><tr><td>Rechazado Sistema Aduana AT</td><td>El despacho se encuentra con DUS AT rechazado por el sistema de Aduana</td><td></td></tr><tr><td>Pend. Ingreso ZP</td><td>El despacho se encuentra pendiente de ingreso a zona primaria</td><td></td></tr><tr><td>Pend. Zarpe Nave</td><td>El despacho se encuentra con vía marítima y pendiente de zarpe</td><td></td></tr><tr><td>Pend. Legalización</td><td>El despacho se encuentra disponible para legalizar</td><td></td></tr><tr><td>Pend. Aceptación DUS Leg.</td><td>El despacho se encuentra con legalización del DUS presentada</td><td></td></tr><tr><td>Rechazado Sistema Aduana DUS Leg.</td><td>El despacho se encuentra con legalización del DUS rechazada por el sistema de Aduana</td><td></td></tr><tr><td>Pend. Presentación (IVV)</td><td>El despacho se encuentra con DUS legalizado pendiente de presentación IVV</td><td></td></tr><tr><td>Pend. Aduana (IVV)</td><td></td><td></td></tr><tr><td>Pend. Cochilco (IVV)</td><td></td><td></td></tr><tr><td>Rechazado (IVV)</td><td></td><td></td></tr><tr><td>DUS Anulado</td><td></td><td></td></tr><tr><td>Finalizado (IVV)</td><td></td><td></td></tr><tr><td>Finalizado (Legalizado)</td><td></td><td></td></tr></tbody></table>

{% hint style="warning" %}
Los despachos que se encuentren anulados, no obtendrán ninguna modificación del estado DUS y los despachos que se encuentren finalizados, solo podrá obtener una modificación del estado DUS si cambia la modalidad de venta.
{% endhint %}

### Vistas

Las vistas se encuentran definidas de acuerdo al perfil del usuario para que de esta manera, puedan gestionar los despachos de manera más óptima.

<table><thead><tr><th>Vistas</th><th>Descripción</th><th data-hidden></th></tr></thead><tbody><tr><td>Mis DUS Pendientes</td><td>Despachos asignados al usuario</td><td></td></tr><tr><td>Pendientes DUS AT</td><td>Despachos pendientes con estados: Pend. Presentación DUS AT, Pend. Aceptación DUS AT, Rechazado Sistema Aduana AT</td><td></td></tr><tr><td>Pendientes Ingreso ZP</td><td>Despachos pendientes con estado: Pend. Ingreso ZP.</td><td></td></tr><tr><td>Pendientes Aforo</td><td>Despachos pendientes con estado: Pendiente Aforo</td><td></td></tr><tr><td>Pendientes Legalización</td><td>Despachos pendientes con estados: Rechazado Sistema Aduana DUS Leg., Pend. Aceptación DUS Leg., Pend. Legalización, Pend. Zarpe Nave </td><td></td></tr><tr><td>Pend. Rev. Doc. DUS Leg.</td><td>Despachos pendientes con estado: Pend. Rev. Doc. DUS</td><td></td></tr><tr><td>Pendientes IVV</td><td>Despachos pendientes con estados: Rechazado (IVV), Pend. Presentación (IVV), Pend. Aduana (IVV), Pend. Cochilco (IVV)</td><td></td></tr><tr><td>Pendientes IVV (Agencia)</td><td>Despachos pendientes con estados: Rechazado (IVV), Pend. Presentación (IVV), Pend. Aduana (IVV), Pend. Cochilco (IVV)</td><td></td></tr><tr><td>Pendientes IVV (Cliente)</td><td>Despachos pendientes con estados: Rechazado (IVV), Pend. Presentación (IVV), Pend. Aduana (IVV), Pend. Cochilco (IVV)</td><td></td></tr><tr><td>DUS en Curso</td><td>Despachos pendientes con estados distintos a Finalizado y Anulado</td><td></td></tr><tr><td>DUS Finalizados (Leg.)</td><td>Despachos Finalizados con el estado: Finalizado (Legalizado)</td><td></td></tr><tr><td>DUS Finalizados (IVV)</td><td>Despachos Finalizados con el estado: Finalizado (IVV)</td><td></td></tr><tr><td>DUS Finalizados (Manualmente)</td><td>Despachos Finalizados con el estado: Finalización Manual</td><td></td></tr><tr><td>DUS Anulados</td><td>Despachos Anulados con el estado: DUS Anulado.</td><td></td></tr></tbody></table>

### Gestión Documental

Dentro del módulo DUS se encuentra el módulo Documentos donde se realiza toda la gestión documental del despacho, el cual resulta de las combinaciones de los estados de los registros, según lo definido por la agencia.

A continuación se muestra una tabla con los estados que se le van asignando a los registros

<table><thead><tr><th>Estado Documento</th><th>Descripción</th><th data-hidden></th></tr></thead><tbody><tr><td>Por Recibir</td><td>Aplica a los registros creados pero que no tienen documentos cargados.</td><td></td></tr><tr><td>Conforme</td><td>Aplica a los registros que se encuentran validados por el ejecutivo y están aprobados.</td><td></td></tr><tr><td>No Conforme</td><td>Aplica a los registros que luego de ser revisados por el ejecutivo, se encuentran rechazados</td><td></td></tr><tr><td>Carpeta Electrónica</td><td>Todo registro que es creado desde carpeta electrónica</td><td></td></tr><tr><td>Por Revisar</td><td>Aplica a los registros que se les ha cargado un documento pero no ha sido validado por el ejecutivo</td><td></td></tr><tr><td>Doc. Complementario</td><td>No influye en el estado documental</td><td></td></tr></tbody></table>

A continuación se muestra una tabla con los estados que resultan, luego de que el robot calcula las combinaciones de los estados de los registros.

<table><thead><tr><th>Estado Documental</th><th>Descripción</th><th data-hidden></th></tr></thead><tbody><tr><td>Sin Documentos</td><td>No hay documentos cargados a los registros</td><td></td></tr><tr><td>Documentos No Conforme</td><td>No hay registros en el estado Por Recibir y existe al menos un registro en el estado No Conforme</td><td></td></tr><tr><td>Documentos En Revisión</td><td>No hay registros en el estado Por Recibir, no hay registros en el estado No Conforme y al menos hay un registro en el estado Por Revisar</td><td></td></tr><tr><td>Documentos Incompletos</td><td>Los registros tienen documentos cargados pero existe al menos un registro en el estado Por Recibir</td><td></td></tr><tr><td>Documentos Completos</td><td>Todos los registros deben estar en el estado Conforme</td><td></td></tr></tbody></table>

#### Cómo cargar un archivo en un registro para la gestión documental

La forma de cargar un archivo al registro puede ser de varias maneras, por registro, desplazando el documento o por carga masiva de documentos.

<mark style="color:blue;">Por Registro</mark>

1. Pinchar el registro.
2. Seleccionar el campo archivo
3. Subir el archivo

<mark style="color:blue;">Desplazando el documento</mark>

1. Teniendo el documento en el escritorio, disminuir el tamaño de la pantalla de la plataforma de EURUS y arrastrar el documento que está en el escritorio, al ícono de nube. Con ello se carga el documento en el registro.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

Si el registro no está creado, se puede arrastrar al ícono ![](<../.gitbook/assets/image (3) (1).png>) y con eso se carga el registro junto con el documento.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

<mark style="color:blue;">Carga Masiva</mark>

1. Disminuir el tamaño de la pantalla de la plataforma EURUS y seleccionar los archivos que desea cargar, que se encuentran en el escritorio.
2. Arrastrar esos documentos y llevarlos al ícono <img src="../.gitbook/assets/image (4).png" alt="" data-size="line"> con ello se cargan todos los registros con su respectivo documento.

{% hint style="info" %}
Todos los documentos cargados, quedarán en el Estado Documento "Por Revisar".
{% endhint %}
