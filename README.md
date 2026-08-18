# ConectaNegocio — Entrega M1

> Compara, conversa y haz seguimiento sin cambiar de plataforma.

ConectaNegocio es una plataforma web para centralizar el abastecimiento entre pequeños comercios y sus proveedores. Este repositorio contiene la entrega **M1 — Problem Statement + Prototype** del curso Desarrollo de Aplicaciones Web de la Universidad de La Sabana.

## Enlaces de la entrega

- [Prototipo en GitHub Pages](https://josealejandromelom.github.io/M1---Desarrollo-Web---C1/)
- [Repositorio](https://github.com/JoseAlejandroMeloM/M1---Desarrollo-Web---C1)
- [Diseño de interfaz en Figma](https://www.figma.com/design/i0LHQGczrAGr6AqProBqJV/Proyecto-DSAW?node-id=0-1&t=ZS6t7uOzXtOQ8xty-1)
- [Wireframes y estados en Figma](https://www.figma.com/make/3drdhe0Y3KiYPeWRJ75b4X/Wireframe-Ofertas-Estado-Vac%C3%ADo?t=YKTxr7a9hPD7wUPm-1)
- [Matriz de pantallas y recorrido](./WIREFRAMES.md)

## Problema real

Los administradores de pequeños comercios que compran productos a varios proveedores no cuentan con un espacio centralizado para comparar ofertas equivalentes, conservar la conversación de cada negociación y consultar el avance de sus pedidos y entregas.

El problema fue identificado a partir del caso real de **Sol y Luna**, una papelería de Chía. Su administradora debe contactar a cada proveedor por separado y comparar manualmente variables como precio, referencia, presentación, cantidad mínima, disponibilidad, forma de pago y tiempo de entrega. Una papelería puede manejar pedidos cercanos a 1.500 productos, organizados en lotes y distribuidos entre distintos proveedores.

La información queda repartida entre WhatsApp, llamadas, facturas, notas y una plataforma de ventas que administra el inventario del negocio, pero no permite comparar ni gestionar la información de los distribuidores. Esto consume tiempo, dificulta reconocer referencias parecidas y aumenta el riesgo de perder las condiciones acordadas o desconocer el estado de una entrega.

## Usuarios objetivo

### Comerciante o administrador del negocio

Propietarios y administradores de papelerías u otros pequeños comercios que compran productos recurrentemente a varios proveedores. La administradora de Sol y Luna es el usuario de referencia inicial.

### Proveedor o distribuidor

Empresas que publican ofertas, responden consultas, confirman pedidos y comunican el avance de preparación y entrega a sus clientes comerciales.

## ¿Por qué una aplicación web?

- **Una hoja de cálculo no permite una colaboración comercial completa.** Puede almacenar precios, pero no permite que cada proveedor administre sus ofertas, responda conversaciones y actualice pedidos desde una cuenta con permisos propios.
- **WhatsApp no organiza la información alrededor de la compra.** Las conversaciones quedan mezcladas y no relacionan estructuradamente cada producto, oferta, pedido y entrega.
- **La plataforma de inventario existente no compara distribuidores.** El comercio todavía debe revisar manualmente presentaciones, compras mínimas, precios y tiempos de entrega.
- **Una aplicación exclusivamente móvil limita el trabajo administrativo.** La web funciona en computador, tableta y teléfono, y facilita revisar catálogos y pedidos grandes en una pantalla amplia.
- **Comerciante y proveedor necesitan la misma información actualizada.** La aplicación web centraliza ofertas, conversaciones, pedidos e historial para que ambas partes compartan contexto.

## Propuesta de valor

ConectaNegocio integra tres funciones en un solo recorrido:

1. **Comparación:** alinea precio, presentación, compra mínima, disponibilidad y entrega de diferentes proveedores.
2. **Comunicación:** conserva un chat asociado a una oferta o pedido específico.
3. **Seguimiento:** muestra el avance del pedido y permite registrar entregas parciales o totales.

## Recorrido demostrable de M1

1. El comerciante consulta y filtra ofertas.
2. Selecciona dos o más opciones y abre el comparador.
3. Inicia una conversación contextual con el proveedor elegido.
4. Crea un pedido ficticio sin perder la información acordada.
5. El proveedor consulta el pedido y actualiza su estado.
6. El comerciante revisa la línea de tiempo y confirma la recepción.

El prototipo usa datos simulados y `localStorage`; no crea compras reales ni envía información a un servidor.

## Roles y permisos

| Acción | Comerciante | Proveedor |
|---|:---:|:---:|
| Buscar productos y comparar ofertas | Sí | Consulta limitada |
| Iniciar conversaciones y crear pedidos | Sí | Responde y confirma |
| Confirmar la recepción | Sí | No |
| Crear o editar sus propias ofertas | No | Sí |
| Actualizar preparación, envío y entrega | No | Sí |
| Modificar información de otro proveedor | No | No |

En M1 estos permisos se representan mediante pantallas y controles diferenciados. En M3 deberán verificarse también en el backend.

## Historias de usuario

- Como administrador de un pequeño negocio, quiero comparar ofertas para escoger la mejor combinación de precio, cantidad y entrega.
- Como administradora de una papelería, quiero distinguir referencias y presentaciones similares para pedir el producto correcto.
- Como comerciante, quiero conversar desde una oferta o pedido para conservar el contexto de la negociación.
- Como comerciante, quiero consultar el estado de cada pedido para saber qué está pendiente, en tránsito o entregado.
- Como proveedor, quiero actualizar mis ofertas y pedidos para que mis clientes reciban información vigente.

## Alcance de M1

- Problem statement sustentado en un usuario real.
- Wireframes de las pantallas principales y sus estados.
- Prototipo estático navegable con HTML semántico, CSS y JavaScript.
- Simulación de los tres flujos centrales con datos ficticios.
- Diseño responsive, accesible y publicado en GitHub Pages.

## Fuera del alcance inicial

Inventario integral, punto de venta, facturación electrónica, pagos reales, contabilidad, lectura automática de facturas, predicción de inventario, reportes avanzados y aplicación móvil nativa.

La regla de alcance es: si una función no mejora directamente la comparación, la comunicación o el seguimiento, debe quedar para una versión futura.

## Equipo

- Catalina Vega Romero
- Jose Alejandro Melo Murcia
- Alejandro Caycedo
- Sebastián Franco Umbacia

Las contribuciones individuales se documentan mediante el historial real de Git y los archivos entregados por el equipo.

## Tecnologías

- HTML5 semántico.
- CSS responsive con variables, Grid y Flexbox.
- JavaScript moderno sin frameworks.
- `localStorage` para conservar el estado demostrativo.
- Figma para wireframes y diseño.
- GitHub y GitHub Pages para colaboración y publicación.

## Ejecutar localmente

Los módulos de JavaScript necesitan un servidor HTTP local. Desde la carpeta del proyecto se puede usar cualquier servidor estático, por ejemplo la extensión Live Server de VS Code. Luego se abre `index.html` desde la dirección que muestre el servidor.

## Datos y privacidad

Sol y Luna es el caso real que fundamenta el problema. Los nombres de perfiles, proveedores, productos, precios, mensajes, pedidos y actividades mostrados dentro del prototipo son ficticios y se utilizan exclusivamente con fines académicos.

## Entrega

- **Hito:** M1 — Problem Statement + Prototype.
- **Fecha límite:** 18 de agosto de 2026, 7:00 a. m. (hora de Colombia).
- **Curso:** Desarrollo de Aplicaciones Web, Universidad de La Sabana.
