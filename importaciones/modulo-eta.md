---
description: >-
  El presente Módulo se compone por un listado de naves que agrupan despachos en
  curso y que requieren de la actualización de la Fecha ETA.
---

# Módulo ETA

## ¿Cómo buscar una nave? :mag:&#x20;

Para filtrar una nave se debe considerar lo siguiente:

1. El despliegue  de información es exclusivamente por sucursal, siendo indispensable seleccionarla previamente con el filtro manual, ubicado en la parte superior izquierda del Módulo.
2. Un vez seleccionada la sucursal, se puede filtrar la nave en la barra de búsqueda del módulo, ya sea por Nombre, Manifiesto, Puerto de Desembarque o Fecha ETA.

## Ordenamiento :arrow\_down:&#x20;

Las naves se ordenan por Fecha ETA, **desde la más antigua hasta la más reciente.**  De esta manera, las naves sin fecha ETA se ubican al principio.

## Actualización Fecha ETA :date:&#x20;

Al modificar la Fecha ETA de una de las naves, todos los despachos pertenecientes a tal agrupación, obtendrán la Fecha ETA actualizada, es decir, la recién ingresada por el usuario.

{% hint style="warning" %}
Si la agrupación de despachos carece de Nave, Manifiesto o Puerto de Desembarque, el campo **Fecha ETA** permanecerá **inhabilitado** para editar.&#x20;
{% endhint %}

### Control de frecuencia de actualización de la Fecha ETA&#x20;

En el campo **Días Última Act.** se visualiza los días transcurridos desde la última actualización de la Fecha ETA. **** El campo se destaca con color de acuerdo a los siguientes parámetros:

* **Verde,** si no ha transcurrido un día desde la última actualización.
* **Rosado,** si ha transcurrido más de 1 día desde la última actualización.

{% hint style="success" %}
Se espera que el usuario mantenga el campo destacado en **verde.**&#x20;
{% endhint %}

## **Categorización de despachos por nave**  :dividers:&#x20;

Los siguientes campos contabilizan la cantidad de despachos por nave, según etapa. Los estados DIN que se consideran por etapa son los siguientes:

| **Etapa**     | **Estado DIN**                                                                              |
| ------------- | ------------------------------------------------------------------------------------------- |
| **Ejecutivo** | Documentos en Revisión y Documentos Incompletos.                                            |
| **Pedidor**   | <p>Pendiente Presentación DIN, Pendiente Aceptación DIN y Rechazado Sistema Aduana.<br></p> |
| **Pago**      | Pendiente Pago Impuestos (GCP).                                                             |
| **Retiro**    | Pendiente Retiro.                                                                           |

## ¿Cómo acceder a los despachos contenidos en una nave?  :arrow\_upper\_left:&#x20;

Basta con presionar uno de los campos Ejecutivo, Pedidor, Pago o Retiro para obtener los despachos contenidos en la nave, ya que funcionan como botones que redirigen al Módulo DIN y filtran las operaciones por nave.

## ¿Por qué no puedo editar la Fecha ETA de una nave? :no\_entry\_sign:&#x20;

Las naves se conforman por una agrupación de despachos en curso que coinciden con el valor de los campos Nave, Manifiesto y Puerto de Desembarque. Entonces, **si los despachos se encuentran agrupados como una nave y no tienen completo uno o más de los 3 campos mencionados**, el campo permanecerá inhabilitado hasta que se obtenga la totalidad de la información.

{% hint style="info" %}
Si la nave posee fecha de arribo, el campo Fecha ETA se encontrará inhabilitado.&#x20;
{% endhint %}



