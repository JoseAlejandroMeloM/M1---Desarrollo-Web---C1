# Problem Statement — ConectaNegocio

## ¿Cuál es el problema?

Los administradores de pequeños comercios (por ejemplo, una papelería de
barrio) que compran productos a varios proveedores no cuentan con un
espacio centralizado para comparar ofertas equivalentes, conservar la
conversación asociada a cada negociación y consultar el avance de sus
pedidos y entregas.

## ¿A quién afecta?

- **Comerciantes:** administradores o propietarios de pequeños comercios
  que compran productos a varios proveedores de forma recurrente.
- **Proveedores/distribuidores:** publican productos, reciben pedidos de
  esos comercios y gestionan su preparación, despacho y entrega.

## ¿Por qué es un problema?

- La información necesaria para abastecer el negocio está repartida
  entre llamadas, WhatsApp, facturas y notas sueltas.
- Comparar ofertas manualmente consume tiempo y es propenso a error:
  productos semejantes pueden tener descripciones ambiguas o
  inconsistentes entre proveedores.
- WhatsApp organiza las conversaciones por contacto, no por producto,
  oferta o pedido — comparar proveedores implica saltar entre chats y
  perder contexto.
- No existe una vista central del estado de un pedido ni de las
  entregas parciales, lo que obliga a preguntar repetidamente.

## ¿Qué necesidad identificaron?

A partir de una conversación con la administradora de una papelería que
trabaja con numerosos productos y varios proveedores, se identificó que
necesita: comparar condiciones de distintos proveedores en un solo
lugar, mantener la conversación comercial ligada a la negociación
específica, y tener visibilidad compartida del estado de un pedido sin
tener que preguntar de nuevo.

## Objetivos y requerimientos principales de la solución

1. Comparar ofertas de distintos proveedores para un mismo producto,
   con atributos equivalentes alineados (precio, presentación, compra
   mínima, tiempo de entrega).
2. Chat interno contextual, vinculado a una oferta o pedido específico.
3. Seguimiento del pedido con estados definidos e historial, incluyendo
   entregas parciales.
4. Dos roles con permisos distintos — comerciante y proveedor —
   verificados en el backend, no solo en la interfaz.
5. Explícitamente fuera de alcance: pagos, inventario, facturación,
   punto de venta.