---
title: Plan de prueba "minimo" (repositorio local en H2 sin autenticacion)
plancode: VC00PLAN000
srcpath: "casos/VC00/plans/planVC00PLAN000.md"
---

{% include es/header.md %}

# {{ page.title }}

Este plan de prueba contiene test para verificar la funcionalidad minima de VCSGis sobre 
un repositorio local en H2 que no tiene la autenticacion de usuarios activada.

Comprueba:
1. Que se crea un repositorio.
1. Que se crea una copia de trabajo.
1. Que se pueden añdir a la copia de trabajo capas, commitarlas y hacer checkout de ellas.

Casos de prueba:
1. ${check} [Crear repositorio sobre H2](../CR00/CP000/testVC00CR00CP000.md).
1. ${check} [Crear copia de trabajo asoiada a un repositorio local en H2](../CW00/CP000/testVC00CW00CP000.md).
1. ${check} [Añadir capa a la copia de trabajo (add)](../AD00/CP000/testVC00AD00CP000.md).
1. ${check} [Subir capa al repositorio local (commit)](../SY00/CP000/testVC00SY00CP000.md).
1. ${check} [Descargar capa a la copia de trabajo (checkout)](../CO00/CP000/testVC00CO00CP000.md).


{% include es/footer.html %}


