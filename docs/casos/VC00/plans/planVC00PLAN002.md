---
title: Plan de prueba "basico" (repositorio remoto en H2 con autorizacion)
plancode: VC00PLAN002
srcpath: "casos/VC00/plans/planVC00PLAN002.md"
---

{% include es/header.md %}

# {{ page.title }}

Este plan de prueba contiene test para verificar la funcionalidad basica de VCSGis sobre 
un repositorio remoto en H2 con la autenticacion y autorizacion de usuarios activada.

Comprueba:
1. Que se crea un repositorio.
1. Que se crea una copia de trabajo.
1. Que se pueden añdir a la copia de trabajo capas, commitarlas y hacer checkout de ellas.

1. Que se se pueden crear leyendas asociadas a una capa y se cargan automaticamente al cargarla en una vista.

1. Que la integración con el marco de topologia funciona, pudiendose registrar planes
  de topologia en el repositorio, asociarlos a tablas de este, y pasarlos antes de subir cambios
  al repositorio.

{% comment %}

1. Que se se detectan correctamente los conflictos al editar simultaneamente desde dos usuario una capa del repositorio.

1. Que se pueden definir modelos de datos y se puede cargar en los puestos.

{% endcomment %}


Casos de prueba:
1. ${check} [Crear repositorio sobre H2](../CR00/CP001/testVC00CR00CP001.md).
1. ${check} [Crear copia de trabajo](../CW00/CP002/testVC00CW00CP002.md).

1. ${check} [Añadir capa a la copia de trabajo (add)](../AD00/CP002/testVC00AD00CP002.md).
1. ${check} [Subir capa al repositorio local (commit)](../SY00/CP002/testVC00SY00CP002.md).
1. ${check} [Descargar capa a la copia de trabajo (checkout)](../CO00/CP002/testVC00CO00CP002.md).

1. ${check} [Asociar leyenda a una capa](CP003/testVC00RE00CP003.md).

1. ${check} [Cargar un plan topologico en el repositorio](../TP00/CP000/testVC00TP00CP000.md).
1. ${check} [Asociar un plan topologico a una capa](../TP00/CP001/testVC00TP00CP001.md).
1. ${check} [Subir cambios en una capa con un plan topologico (que no pasen el plan)](../TP00/CP002/testVC00TP00CP002.md).

{% comment %}

1. ${check} [Definir y descargar un modelo de datos](CP003/testVC00RE00CP003.md).

{% endcomment %}

{% include es/footer.html %}
