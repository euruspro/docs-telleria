# Aforo DIN

Los datos se consultan en la página web: h[ttp://comext.aduana.cl:7001/DespachadoresWeb/begin.do](http://comext.aduana.cl:7001/DespachadoresWeb/begin.do)

### Condiciones que debe cumplir un despacho para ser consultado por el robot en Aduana

1. El despacho debe tener número de manifiesto
2. El despacho debe tener fecha de aceptación
3. El despacho no debe tener fecha de retiro

{% hint style="info" %}
**Nota 1**: La consulta se realiza hasta que el despacho obtenga la fecha de retiro.

**Nota 2**: Cada vez que se genera un registro de Aforo en el módulo, se debe rescatar el comprobante "Selección de Aforo", el cual se visualiza en EURUS, en el formulario del registro, en el campo Comprobante y en el tab de documentos del despacho.
{% endhint %}

### Vistas

<table><thead><tr><th>Vista</th><th>Estado</th><th data-hidden></th></tr></thead><tbody><tr><td>Aforos Pendientes</td><td>Aforo Pendiente</td><td></td></tr><tr><td>Aforos Realizados</td><td>Aforo Realizado AS, Aforo Realizado con Obs No As, Aforo Realizado sin Obs No AS, Aforo Realizado con Obs AS, Finalización Manual Aforo, Aforo Realizado</td><td></td></tr><tr><td></td><td></td><td></td></tr></tbody></table>
