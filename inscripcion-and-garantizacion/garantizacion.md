# Garantización

### Criterio para indicar que un despacho requiere Garantización

1. Debe ser un despacho DIN
2. Vía de transporte debe ser Marítima
3. Tipo de bulto debe ser alguno de los siguientes tipos:
   1. &#x20;'CONT20',&#x20;
   2. 'CONT40',&#x20;
   3. 'REEFER20',&#x20;
   4. 'REEFER40', ó
   5. 'CONTNOESP'
4. La fecha de retiro no debe estar definida.
5. El despacho debe implicar un retiro.

{% hint style="warning" %}
**Advertencia**

En caso de que alguno de los criterios anteriores cambie o deje de cumplir las condiciones, el despacho ya **no requerirá proceso de Garantización**.
{% endhint %}



### Estados de la Garantización

<table><thead><tr><th width="258">Estado</th><th>Descripción</th></tr></thead><tbody><tr><td>Por Garantizar</td><td><strong>Estado por defecto</strong>, se asigna solo cuando el despacho cumple con los criterios para ser garantizado</td></tr><tr><td>Garantizado</td><td></td></tr><tr><td>Carta Garantía</td><td></td></tr><tr><td>Shipper Owned Container (SOC)</td><td>Estado se selecciona manualmente, bajo criterio del usuario de la Agencia.</td></tr><tr><td>Carga Break Bulk</td><td>Estado se selecciona manualmente, bajo criterio del usuario de la Agencia.</td></tr><tr><td>Anulado</td><td></td></tr><tr><td>Por Corregir Garantía</td><td>Se asigna este estado de manera automática, cuando el despacho cambia de <strong>Nombre de Nave, Puerto de Desembarque o Tipo de Bulto</strong>. <br><br><strong>NOTA</strong>: Este estado también puede ser asignado manualmente.</td></tr><tr><td>Rechazado</td><td>Estado que se asigna cuando se crea un registro y el sistema lo rechaza por no cumplir con los <strong>criterios de asignación</strong>.</td></tr></tbody></table>

### Criterios de asignación de Estado Garantización

1. Se verifica que la cantidad Garantizada, sea menor o igual a la cantidad pendiente de Garantizar, en caso contrario, rechaza el registro.
2. Si el registro es del estado Carta Garantía, Garantizado o SOC, se valida que el registro tenga un comprobante cargado, en caso contrario lo rechaza.
3. Al asignar o modificar un estado de garantización, se replica el estado y el registro de garantización a los despachos parciales, si es que aplica

