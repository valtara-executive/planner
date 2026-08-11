# Mapa demostrativo — Plataforma digital de tres negocios

Este repositorio contiene **maquetas visuales de alta fidelidad** para tres
líneas de negocio: una constructora, un despacho de arquitectura con
showroom inmobiliario, y un coworking de espacios para profesionales de la
salud. El objetivo es mostrar el **alcance y flujo funcional** que tendría
cada plataforma antes de construir la versión real.

> ⚠️ **Esto no es un producto terminado.** Son prototipos de navegador sin
> backend, sin base de datos y sin conexión a ningún servidor. Todos los
> nombres de empresa, personas, obras, proyectos, precios y datos que
> aparecen son **ficticios**, generados únicamente para que la demo se vea
> completa y funcional. El inicio de sesión de los paneles internos es
> **simulado**: acepta cualquier usuario y contraseña a propósito, solo para
> poder mostrar cómo se vería el panel una vez dentro — no debe usarse como
> referencia de seguridad ni desplegarse tal cual en producción.

---

## Cómo está organizado

Cada una de las tres marcas tiene tres piezas: un **catálogo público** (lo
que ve cualquier visitante sin iniciar sesión), un **panel de cliente** (lo
que ve alguien ya registrado dando seguimiento a su obra/proyecto/reserva),
y un **panel administrativo interno** (lo que usa el equipo para operar el
negocio).

```
/torreon-constructora/
    catalogo-publico.html      → Catálogo de obras, cotización
    panel-cliente.html         → Seguimiento de obra, bitácora, pagos
    panel-admin.html           → Gestión interna de todas las obras

/arqueo-estudio/
    catalogo-publico.html      → Showroom inmobiliario, proyectos
    panel-cliente.html         → Seguimiento de diseño, mi proyecto
    panel-admin.html           → Gestión interna de proyectos y catálogo

/ile-wellness/
    catalogo-publico.html      → Reserva de espacios, disponibilidad
    panel-cliente.html         → Panel del profesional que renta espacio
    panel-admin.html           → Operación interna del coworking
```

Cada archivo HTML es **autocontenido**: se abre directo en el navegador, sin
instalar nada ni necesitar conexión a un servidor propio (las imágenes se
cargan desde un servicio externo de imágenes de muestra).

---

## Cómo ver la demo

Todas las páginas están publicadas con GitHub Pages, así que basta con abrir
el enlace correspondiente en cualquier navegador (computadora o celular).

**Punto de entrada recomendado:** empieza siempre por el **catálogo
público** de cada marca — es la puerta de entrada real de un visitante.
Desde ahí, el botón de "Iniciar sesión" te lleva conceptualmente al panel
de cliente (en esta demo son archivos independientes, así que se abren por
separado).

Para el panel de cliente y el panel administrativo, en la pantalla de login
puedes escribir **cualquier usuario y cualquier contraseña** — está
diseñado a propósito para entrar sin fricción y mostrar cómo se ve la
plataforma por dentro.

---

## Qué sí funciona en estas maquetas

Aunque no hay backend real, cada panel tiene lógica funcional dentro del
navegador:

- Filtros y búsqueda en tiempo real sobre los catálogos
- Favoritos y comparador de proyectos/espacios/obras
- Formularios con validación y confirmación
- Notificaciones que aparecen solas mientras navegas, simulando actividad
  en tiempo real
- Chat de ejemplo con respuestas automáticas
- Gráficos, calendarios y tableros con datos de muestra generados en el
  propio código

## Qué NO incluyen (a propósito)

- Base de datos o persistencia real de la información
- Autenticación real de usuarios
- Procesamiento real de pagos
- Envío real de correos, mensajes o notificaciones
- Conexión entre las distintas páginas/paneles (cada archivo es
  independiente)

---

## Próximo paso

Este mapa demostrativo sirve como base de discusión para definir el alcance
real antes de construir la plataforma definitiva desde cero, con nombre de
marca real, backend, base de datos y autenticación seguros.
