# Historias de Usuario – Módulo de Sincronización de Stock

Las historias de usuario describen qué necesita cada persona que va a usar el sistema, con el formato:
**Como** [usuario], **quiero** [funcionalidad], **para** [beneficio].

Cada historia tiene criterios de aceptación, que indican cuándo se considera terminada.

---

## HU-01 – Stock real en la tienda online

**Como** responsable de la tienda online (Área de Marketing),
**quiero** que el stock de armazones publicado en Tiendanube se actualice automáticamente con el stock de Moebius,
**para** no vender productos que no están disponibles físicamente.

**Criterios de aceptación:**
- Cuando se vende un armazón en una sucursal, el stock en Tiendanube se actualiza en menos de 1 minuto.
- Cuando se vende un armazón por la web, el stock se descuenta también en Moebius.
- Si un armazón queda sin stock, deja de poder comprarse en la tienda online.

**Prioridad:** Alta
**Relación con entregas anteriores:** Meta 1 y Meta 3 de la Entrega 2; entidades `Stock` y `Producto_Tiendanube` de la Entrega 3.

---

## HU-02 – Ubicación del armazón vendido

**Como** encargado del sector de Armazones,
**quiero** ver en qué sucursal y en qué ubicación del depósito está el armazón vendido por la web,
**para** encontrarlo rápido y prepararlo a tiempo para la entrega.

**Criterios de aceptación:**
- Cada venta online muestra la sucursal y la ubicación (estante o caja) del armazón.
- Si el armazón no se encuentra en la ubicación indicada, se puede marcar como "no encontrado" para revisar el stock.

**Prioridad:** Alta
**Relación con entregas anteriores:** caso de la venta de $300.000 (Entregas 1 y 2); campo `ubicacion_deposito` de la entidad `Stock` (Entrega 3).

---

## HU-03 – Registro de sincronizaciones

**Como** responsable del Área de Sistemas,
**quiero** un registro de cada sincronización con su fecha, hora, origen y resultado,
**para** detectar errores rápidamente y controlar que el módulo cumpla las metas del proyecto.

**Criterios de aceptación:**
- Cada sincronización queda guardada con el armazón, el stock anterior y el nuevo, el origen (Moebius o Tiendanube) y el resultado (OK o Error).
- Si una sincronización falla por un corte de conexión, queda pendiente y se vuelve a intentar automáticamente.
- Se puede consultar el historial de un armazón para saber cuándo y dónde cambió su stock.

**Prioridad:** Media
**Relación con entregas anteriores:** medida ante caídas de conexión (Entrega 1); entidad `Registro_Sincronizacion` (Entrega 3).