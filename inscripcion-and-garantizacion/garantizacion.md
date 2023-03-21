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

| Estado                        | Descripción                                                                                                                                                                                                                                                                                                                                                                                                             |
| ----------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Por Garantizar                | **Estado por defecto**, se asigna solo cuando el despacho cumple con los criterios para ser garantizado                                                                                                                                                                                                                                                                                                                 |
| Garantizado                   |                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Carta Garantía                |                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Shipper Owned Container (SOC) |                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Carga Break Bulk              | Se selecciona manualmente, para que deje sin efecto la necesidad de Garantizarción.  Dado que esta carga viene generalmente bajo la descripción "Piezas", pero no sirve este código para utilizarlo como variable de entrada para automatizar esta acción, ya que hay otras cargas sueltas que vienen también bajo la descripción "Piezas", pero que sí deben inscribirse. Por eso la necesidad de la selección manual. |
| Anulado                       |                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Por Corregir Garantía         | <p>Se asigna este estado de manera automática, cuando el despacho cambia de <strong>Nombre de Nave, Puerto de Desembarque o Tipo de Bulto</strong>. <br><br><strong>NOTA</strong>: Este estado también puede ser asignado manualmente.</p>                                                                                                                                                                              |
| Rechazado                     | Estado que se asigna cuando se crea un registro y el sistema lo rechaza por no cumplir con los **criterios de asignación**.                                                                                                                                                                                                                                                                                             |

### Criterios de asignación de Estado Garantización

1. Se verifica que la cantidad Garantizada, sea menor o igual a la cantidad pendiente de Garantizar, en caso contrario, rechaza el registro.
2. Si el registro es del estado Carta Garantía, Garantizado o SOC, se valida que el registro tenga un comprobante cargado, en caso contrario lo rechaza.

