# Módulo de Sincronización de Stock – Óptica Central

**Trabajo Práctico Integrador – Organización Empresarial**
Tecnicatura Universitaria en Programación a Distancia (TUPaD) – Universidad Tecnológica Nacional

|---|---|
| **Alumno** | Matías Salazar |
| **Docente Titular** | Prof. Mario Raúl López |
| **Docente Tutor** | Franco Corts-Romeo |
| **Tablero de gestión** | [GitHub Projects – Óptica Central](PEGAR_ACA_EL_LINK_DEL_TABLERO) |

## Descripción del proyecto

**Óptica Central** es una cadena de ópticas de la provincia con 10 sucursales, un taller de armado propio y una tienda online desarrollada en **Tiendanube**. Para la gestión diaria, todas las sucursales usan el software **Moebius** (facturación, clientes, ventas).

**El problema:** la tienda online funciona como una "sucursal aparte" y su stock no está conectado con el de Moebius. Esto ya generó problemas reales, como la venta online de un anteojo de sol de $300.000 que figuraba disponible pero no se encontraba en el depósito al momento de la entrega.

**La propuesta:** un módulo de sincronización de stock que conecte el inventario de armazones de Moebius con la tienda online a través de la API de Tiendanube, para que ambas plataformas muestren el mismo stock en tiempo real. El desarrollo lo lleva el Área de Sistemas junto con el equipo de Moebius, con una implementación gradual que empieza por los armazones más vendidos.

## Modalidad de trabajo

Este trabajo se realizó de forma **individual**. Por eso, la instancia de revisión de los Pull Requests es una **autorrevisión**: antes de cada merge se revisaron los cambios en la pestaña *Files changed*, se dejaron comentarios sobre lo que convenía ajustar y se resolvieron antes de integrar la rama a `main`.

El trabajo se realizó localmente en Visual Studio Code, con una rama por cada parte del proyecto, y los Pull Requests se gestionaron desde GitHub.

## Contenido

- `entregas/`: PDFs de las entregas 1, 2, 3 y la final.
- `diagramas/`: diagramas del proyecto (incluye el BPMN).
- `docs/historias-de-usuario.md`: historias de usuario.
- `docs/indicadores-de-control.md`: indicadores de control.

## Declaración de Uso de IA

Usé Claude como ayuda para entender la consigna, ordenar el repositorio y armar un primer borrador de las historias de usuario, los indicadores y el BPMN.

**Prompts principales:**
- Le compartí la consigna y mis entregas anteriores para organizar qué faltaba hacer en esta etapa.
- Le pedí ideas para armar las historias de usuario y los indicadores a partir del módulo de sincronización.

**Lo que corregí yo:**
- La IA agregó en esta declaración un pedido que yo no había hecho, así que lo saqué y la ajusté a lo que realmente le consulté.
- Consulté con el tutor cómo hacer la revisión de pares trabajando solo.

El caso, los datos de la empresa y las decisiones del proyecto son míos.