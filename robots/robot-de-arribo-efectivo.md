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

Filtra todos los despachos DIN, que tenga como Código de Vía de transporte el "01", no tenga Fecha de Arribo y No  tenga fea de Retiro.
