# Aforo DUS

Los datos se consultan en la página web: h[ttp://comext.aduana.cl:7001/DespachadoresWeb/begin.do](http://comext.aduana.cl:7001/DespachadoresWeb/begin.do)

El robot copia la información del estado Aforo y la copia en el despacho.

### Estados presentes en el módulo

<table><thead><tr><th>Estado</th><th>Descripción</th><th data-hidden></th></tr></thead><tbody><tr><td>Aforo Pendiente</td><td>Se asigna a los registros de Ingreso a ZP que en el campo Tipo Selección, tenga un valor distinto a Sin Examen y que en el campo Estado Ingreso a ZP tenga un valor distinto a Autorizado a Salir</td><td></td></tr><tr><td>Aforo Realizado</td><td>Se asigna a los registros que el campo Tipo Selección tengan un valor distinto a Sin Examen y que el campo Estado Ingreso a ZP tenga un valor igual a Autorizado a Salir</td><td></td></tr><tr><td></td><td></td><td></td></tr></tbody></table>

### Vistas

<table><thead><tr><th>Vista</th><th>Estado</th><th data-hidden></th></tr></thead><tbody><tr><td>Aforos Pendientes</td><td>Aforo Pendiente</td><td></td></tr><tr><td>Aforos Realizados</td><td>Aforo Realizado</td><td></td></tr></tbody></table>

