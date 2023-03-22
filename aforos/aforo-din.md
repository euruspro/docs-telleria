# Aforo DIN

Los datos se consultan en la página web: h[ttp://comext.aduana.cl:7001/DespachadoresWeb/begin.do](http://comext.aduana.cl:7001/DespachadoresWeb/begin.do)

### Condiciones que debe cumplir un despacho para ser consultado por el robot en Aduana

1. El despacho debe tener número de manifiesto
2. El despacho de ser marítimo ó áereo ó terrestre
3. El despacho debe tener fecha de aceptación
4. El despacho no debe tener fecha de retiro

{% hint style="info" %}
**Nota 1**: La consulta se realiza hasta que el despacho obtenga la fecha de retiro.

**Nota 2**: Cada vez que se genera un registro de Aforo en el módulo, se debe rescatar el comprobante "Selección de Aforo", el cual se visualiza en EURUS, en el formulario del registro, en el campo Comprobante y en el tab de documentos del despacho.
{% endhint %}

### Estados presentes en el módulo

<table><thead><tr><th>Estado</th><th>Descripción</th><th data-hidden></th></tr></thead><tbody><tr><td>Aforo Pendiente</td><td>Se asigna cuando el campo Tipo Aforo tiene el valor <strong>Sin Inspección</strong></td><td></td></tr><tr><td>Aforo Realizado AS</td><td>Se asigna cuando el campo Tipo Aforo tiene un valor distinto a <strong>Sin Inspección</strong> y el campo  Resultado está vacío.</td><td></td></tr><tr><td>Aforo Realizado con Obs No As</td><td>Se asigna cuando el campo Tipo Aforo tiene un valor distinto a <strong>Sin Inspección</strong>, <strong></strong> el campo Resultado tiene un valor distinto a <strong>Sin Observaciones y no está vacío</strong>, y el campo Autorización tiene un valor diferente a <strong>Autorizado a Salir</strong>.</td><td></td></tr><tr><td>Aforo Realizado sin Obs No AS</td><td>Se asigna cuando el campo Tipo Aforo tiene un valor distinto a <strong>Sin Inspección</strong>, <strong></strong> el campo Resultado tiene un valor igual a <strong>Sin Observaciones</strong> y el campo Autorización tiene un valor distinto a <strong>Autorizado a Salir</strong></td><td></td></tr><tr><td> Aforo Realizado con Obs AS</td><td>Se asigna cuando el campo Tipo Aforo tiene un valor distinto a <strong>Sin Inspección</strong>, <strong></strong> el campo Resultado tiene un valor distinto a <strong>Sin Observaciones y no está vacío</strong>, y el campo Autorización tiene un valor igual a <strong>Autorizado a Salir</strong>. </td><td></td></tr><tr><td>Finalización Manual Aforo</td><td>Se realiza manualmente, bajo el criterio del usuario de la Agencia</td><td></td></tr><tr><td>Aforo Realizado</td><td></td><td></td></tr></tbody></table>

### Vistas

<table><thead><tr><th>Vista</th><th>Estado</th><th data-hidden></th></tr></thead><tbody><tr><td>Aforos Pendientes</td><td>Se visualizan los aforos con estado Aforo Pendiente</td><td></td></tr><tr><td>Aforos Realizados</td><td>Se visualizan los Aforos con estado: Aforo Realizado AS, Aforo Realizado con Obs No As, Aforo Realizado sin Obs No AS, Aforo Realizado con Obs AS, Finalización Manual Aforo, Aforo Realizado</td><td></td></tr></tbody></table>
