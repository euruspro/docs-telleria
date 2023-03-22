# Inscripción

### Criterio para indicar que un despacho requiere Inscripción

1. Debe ser un despacho DIN
2. La vía de transporte debe ser Marítima (01)
3. El tipo de trámite debe ser Anticipado o Normal
4. El tipo de operación debe estar definido
5. La fecha de retiro no debe estar definida.

{% hint style="warning" %}
**Advertencia**

En caso de que alguno de los criterios anteriores cambie o deje de cumplir las condiciones, el despacho ya **no requerirá proceso de Inscripción**.
{% endhint %}

### Estados de Inscripción

<table><thead><tr><th>Estado </th><th>Descripción</th><th data-hidden></th></tr></thead><tbody><tr><td>Por Inscribir Directo</td><td><strong>Estado por defecto</strong>, se asigna solo cuando el despacho cumple con los criterios para ser garantizado</td><td></td></tr><tr><td>Inscrito Directo</td><td></td><td></td></tr><tr><td>Por Inscribir Pronto Retiro</td><td>Estado se selecciona manualmente, bajo criterio del usuario de la Agencia.</td><td></td></tr><tr><td>Inscrito Pronto Retiro</td><td></td><td></td></tr><tr><td>Por Inscribir Convenio Alm.</td><td></td><td></td></tr><tr><td>Inscrito Convenio Alm.</td><td></td><td></td></tr><tr><td>Por Corregir Inscripción</td><td></td><td></td></tr><tr><td>Indirecto</td><td></td><td></td></tr><tr><td>Anulado</td><td></td><td></td></tr><tr><td>Rechazado</td><td></td><td></td></tr></tbody></table>

### Criterios de asignación de Estado Inscripción

1. Se verifica que la cantidad Inscrita, sea menor o igual a la cantidad pendiente de Inscribir, en caso contrario, rechaza el registro.
2. Si el registro es del estado Inscrito Directo, Inscrito Pronto Retiro, Inscrito Convenio Alm., se valida que el registro tenga un comprobante cargado, en caso contrario lo rechaza.
3. Al asignar o modificar un estado de inscripción, se replica el estado y el registro de inscripción a los despachos parciales, si es que aplica
