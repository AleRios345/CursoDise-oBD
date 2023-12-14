# Carreras

## Listado de Entidades

### carreras  **(ED)**

- carrera_id **(PK)**
- nombre
- tipo_carrera **(FK)**
- fecha
- tiempo
- mejor_tiempo
- altitud
- lugar
- pais **(FK)**
- foto


### tipos_carreras **(EC)**

- tipo_carrera_id **(PK)**
- descripción
- distancia **(UQ)**

### paises **(EC)**

- pais_id **(PK)**
- nombre

## Relaciones

1. Una **carrera** _pertenece_ a un **tipo de carrera** (_1 a 1_).
1. Una **carrera** se _corre_ en un **pais**. (_1 a 1_).

## Diagramas 

### Modelo Entidad - Relación

![Modelo Entidad - Relación](./DiagramaModeloER.png)

### Modelo Relacional de la base de Datos

![Modelo Relacional de la base de Datos](./DiagramaModeloRelacionalBD.drawio.png)

## Reglas de negocio

### carreras

1. Crear el registro de una carrera.
1. Leer el registro de una(s) carrera(s) dada una condición en particular.
1. Leer todos los registros de la entidad carreras.
1. Actualizar los datos de una carrera.
1. Eliminar los datos de una carrera dada una condición en particular.

### tipos_carreras 

1. Crear el registro de un tipo de carrera.
1. Leer el registro de uno(s) tipo(s) carrera(s) dada una condición en particular.
1. Leer todos los registros de la entidad tipos carrerass.
1. Actualizar los datos de un tipo de carrera dada una condición en particular.
1. Eliminar los datos de una carrera dada una condición en particular.

### paises 

1. Crear el registro de un pais.
1. Leer el registro de uno(s) pais(es) dada una condición en particular.
1. Leer todos los registros de la entidad pais.
1. Actualizar los datos de un pais dada una condición en particular.
1. Eliminar los datos de un pais dada una condición en particular.