## Bloques de comando

Todos los pasos para construir un sistema de lobby y efectos visuales.

### Indice:

[Delimitacion](https://github.com/JustTinajero/PokeMapSteps/blob/main/commandblocks.md#paso-1 "Atajo al paso 1")

[Borde del lobby](https://github.com/JustTinajero/PokeMapSteps/blob/main/commandblocks.md#paso-2 "Atajo al paso 2")

[Proteccion del lobby](https://github.com/JustTinajero/PokeMapSteps/blob/main/commandblocks.md#paso-3 "Atajo al paso 3")

[Anti spawn de mobs](https://github.com/JustTinajero/PokeMapSteps/blob/main/commandblocks.md#paso-4 "Atajo al paso 4")

[Paso 5](https://github.com/JustTinajero/PokeMapSteps/blob/main/commandblocks.md#paso-5 "Atajo al paso 5")

[Paso 6](https://github.com/JustTinajero/PokeMapSteps/blob/main/commandblocks.md#paso-6 "Atajo al paso 6")

### Proteccion de Lobby:
Para esto es necesario utilizar unos cuantos comandos y delimitr la zona del lobby.

Los comandos que se usaran son: /fill y /give

#### Paso 1: Delimitacion

Hay que delimitar la zona del hub por la ultima capa del mundo, exactamente en la ultima capa de bedrock, para esto es necesario delimitar la zona del lobby por la parte de encima del mundo, y en cada esquina contraria hay que excavar hasta la capa de la de bedrock e intentar copear la delimitacion de la parte superior, para esto ya deberiamos tener ubicadas las esquinas para que sea mas sencillo.

#### Paso 2: Lobby Border

Una vez delimitado el cuadro, hay que rellenar las lineas que marcan la delimitacion con bloques "border", los cuales se obtienen con el comandos "/give @s border_block".

#### Paso 3: Lobby Protection

Una ves marcado el borde del lobby, hay que rellenar el interior por la misma capa de bedrock con bloques deny, para que no tengan permitido colocar o romper bloques del mismo, para esto utlizaremos el comando /fill, de la siguiente forma, "/fill x y z x y z deny" las primeras coordenadas son de una esquina de la delimitacion, y las segundas la esquina opuesta, con esto ya deberia haber un cuadrado marcado con las lineas exteriores con bloques border.

#### Paso 4:

Para evitar el spawn de mobs, y que este este habilitado en otras zonas del mapa, como excluyendo el lobby, hay que teletransportar las entidades que no sean jugadores u npcs a una zona, y matarlos ahi mismo, para que no influya el drop de estos mobs en el lobby.

Para esto ocupamos usar unos cuantos bloques de comando con repeticion siempre activa, los cuales son:

##### 1: Este es el tp para entidades a una zona a la que los jugadores no pueden acceder, por ejemplo debajo del lobby.

/tp @e[type=!npc,type=!player] x y z

##### 2: Este es el bloque de comando que eliminara las entidades que sean teletransportadas a la zona no accesible. (Este debe estar ubicado justo debajo de las coordenadas donde se le teletransportara a las entidades.)

/kill @e[r=2,type=item,type=!player]

#### Paso 5:

#### Paso 6:
