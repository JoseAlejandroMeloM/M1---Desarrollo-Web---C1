# PRD — ConectaNegocio

## Problema
Los comerciantes de barrio (ej. una papelería) no tienen una forma eficiente
de comparar ofertas entre proveedores ni de hacer seguimiento a sus pedidos.
Hoy lo resuelven por WhatsApp o llamadas sueltas, sin trazabilidad ni
comparación real de precios/condiciones.

## Por qué una aplicación web (no hoja de cálculo, no app existente)
- Una hoja de cálculo no soporta chat en tiempo real ni actualización de
  estado de pedido por ambas partes a la vez.
- No existe una app dedicada a este nicho (comerciante de barrio ↔
  proveedor pequeño) con comparación + chat + seguimiento en un solo flujo;
  las soluciones B2B existentes apuntan a grandes cadenas.
- Se necesitan 2 roles con permisos distintos y persistencia de datos entre
  sesiones, algo que una hoja de cálculo o un chat genérico no ofrecen.

## Roles y permisos
- **Comerciante**
  - Ve y compara ofertas de proveedores
  - Inicia chat con un proveedor
  - Crea un pedido y consulta su estado
  - No puede publicar ofertas ni cambiar el estado de un pedido
- **Proveedor**
  - Publica y edita sus ofertas
  - Responde en el chat
  - Actualiza el estado del pedido (recibido → en preparación → enviado)
  - No puede ver ni editar pedidos de otros proveedores

## Funcionalidades núcleo (de principio a fin)
1. **Comparación de ofertas** — el comerciante filtra/busca ofertas de
   varios proveedores y ve precio, condiciones y disponibilidad en una
   sola vista.
2. **Chat contextual** — desde una oferta específica, el comerciante abre
   un chat con ese proveedor; el mensaje queda vinculado a la oferta, no
   suelto.
3. **Seguimiento de pedido** — el comerciante confirma un pedido desde el
   chat/oferta, y ve el estado actualizado en tiempo real conforme el
   proveedor lo mueve por las etapas.

## Fuera de alcance (explícito)
- Pagos en línea
- Gestión de inventario
- Facturación electrónica

## Estado actual (M1)
- Prototipo estático (landing + páginas de ofertas) construido
- Wireframes en Figma: pendiente completar hasta 15+ pantallas
  (flujo comparar → chat → pedido → seguimiento aún no navegable de
  principio a fin en el HTML)
