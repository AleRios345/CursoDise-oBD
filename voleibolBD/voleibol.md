# Diseño de Base de datos "_Torneo Voleibol_"

## Listado de entidades

### equipos_torneo **(ED)**

- equipo_id **(PK and FK)**
- equipo_nombre 
- torneos_ganados
- pais **(FK)**
- foto

### jugadores **(ED)**

- equipo_jugador_id **(PK)**
- apodo **(PK)**
- nombre **(PK)**
- edad 
- posicion **(FK)**
- pais **(FK)**


### posiciones **(EC)**

- posicion_id **(PK)**
- nombre

### pais **(EC)**

- pais_id **(PK)**
- nombre

## Relaciones

1. Un **equipos_torneo** tiene varios **jugadores** (_1 a M_).
1. Un **jugadores** juega en una **posicion** (_M a 1_).
1. Un **jugadores** pertenece a un **pais** (_M a 1_).
1. Un **equipos_torneo** pertenece a un **pais** (_M a 1_).

## Diagramas

### Modelo Entidad-Relacion Voleibol
![Modelo Entidad-Relacion Voleibol](./diagramasBD/DiagramaERVoleibol.png)

### Modelo Relacional de la Base de Datos
![Modelo Relacional de la Base de Datos Voleibol](./diagramasBD/ModeloRelacionalVolBD.png)

## Reglas del negocio
1. Regla 1