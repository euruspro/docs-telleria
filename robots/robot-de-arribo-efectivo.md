---
description: >-
  Este robot se encarga de obtener la fecha de Arribo de una nave desde la
  página de Aduana (Manifestación Marítima)
---

# Robot de Arribo Efectivo

## Link de consulta

[http://comext.aduana.cl:7001/ManifestacionMaritima](http://comext.aduana.cl:7001/ManifestacionMaritima)

## ¿Cada cuando se ejecuta?

El robot, se ejecuta cada 5 minutos de Lunes a Domingo.

## ¿Que busca?

Filtra todos los despachos DIN, que:

1. Tenga el Código de Vía de transporte  "01",&#x20;
2. No tenga Fecha de Arribo,
3. No  tenga Fecha de Retiro, y
4. Tenga un número de manifiesto definido.

## ¿Qué hace?

Busca manifiesto por manifiesto en la página de Manifestación Marítima y obtiene todos los datos que la página provee, luego guarda en EURUS todos estos datos y los relacionada con todos los despachos que tengan el mismo número de Manifiesto y que a su vez, sean despachos DIN.

Además, el robot ejecuta las siguientes acciones:

* Crea un evento **ED9002 - FECHA ARRIBO EFECTIVO** solo si encuentra una fecha definida en la página de la aduana.

