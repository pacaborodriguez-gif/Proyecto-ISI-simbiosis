# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | [dd/mm/aaaa] |
| Versión | [Versión de trabajo] |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como cliente, quiero poder realizar una búsqueda avanzada, para encontrar recetas según ciertos criterios.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

[Justificación de los resultados útiles que separa la división.]

## US-01

**Título:** Buscar mediante una palabra o frase

Como cliente, quiero poder buscar una receta con una palabra o frase, para poder encontrarla fácilmente.

**Fuentes:** UR-08; UC-21; FR-085; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dada una palabra o frase, cuando se busque, entonces mostrar recetas que la contienen.
- **CA-02.** Dado que no se escriba con las tildes o mayúsculas necesarias, cuando se busque la palabra o frase, entonces se mostrará la receta válida igualmente.
- **CA-03.** Dado que no haya recetas que cumplan los criterios, cuando se busque esa palabra o frase, entonces se mostrará que no hay resultados existentes.

## US-02

**Título:** Buscar por ingredientes incluidos

Como cliente, quiero poder escoger o excluir ciertos ingredientes, para que se muestren recetas que se correspondan con mis necesidades.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que se selecciona el mismo ingrediente para incluirlo e excluirlo, cuando se realice la búsqueda, entonces no se ejecuta la búsqueda hasta que se corrija el error.
- **CA-02.** Dado que ninguna receta contiene los ingredientes, cuando se realice la búsqueda, entonces se indica que no hay resultados coincidentes.
- **CA-03.** Dado que se seleccionan unos ingredientes, cuando se realice la búsqueda, entonces se deberán mostrar todas las recetas que contengan todos los ingrdiente seleccionados.

## US-03

**Título:** Excluir ingredientes

Como cliente de una tienda online, quiero poder excluir ingredientes de mis búsquedas, para que las recetas proporcionadas no los tengan.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, [apartado pertinente].

### Criterios de aceptación

- **CA-01.** Dado que se excluye un ingrediente, cuando se realicen sugerencias de recetas, entonces se mostrarán recetas que no contengan dicho ingrediente.
- **CA-02.** Dado que se han excluido ingredientes anteriormente, cuando se vuelve a los resultados, entonces se conservan los criterios de la última búsqueda.
- **CA-03.** Dado que se selecciona el mismo ingrediente para incluirlo e excluirlo, cuando se realice la búsqueda, entonces no se ejecuta la búsqueda hasta que se corrija el error.

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
