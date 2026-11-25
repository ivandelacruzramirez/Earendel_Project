
README
 · MD


# Earendel Project
 
> Videojuego de realidad virtual de gestión de una granja *cozy* en un planeta desconocido.
> Trabajo de Fin de Grado (TFG) del ciclo de **Desarrollo de Aplicaciones Multiplataforma (DAM)**.
 
**Estado del proyecto:** en desarrollo (versión preliminar de la documentación, 1ª evaluación).
 
---
 
## Descripción
 
Tras una avería, un astronauta queda atrapado en el sistema Earendel. En el único planeta accesible
encuentra una granja abandonada. Para reparar su nave debe recuperarla: cuidar animales, cultivar
alimentos, vender productos y reunir el dinero necesario para comprar las piezas que faltan.
 
Cuando la nave esté lista, el jugador tendrá que decidir entre **volver a su planeta de origen** o
**quedarse en la granja**, que ya se ha convertido en su hogar.
 
La realidad virtual permite observar, coger y manipular objetos y animales directamente con las manos.
 
El nombre hace referencia a *Earendel*, una de las estrellas individuales más lejanas observadas hasta
la fecha, cuyo nombre en inglés antiguo se interpreta como «estrella de la mañana» o «luz naciente».
 
## Características previstas
 
- Gestión de una granja en un mapa delimitado de un único planeta.
- Animales con comportamiento propio (navegación con NavMesh, máquinas de estados, hambre y alimentación).
- Ciclo de cultivo y producción de recursos (lana, huevos, leche, cosechas).
- Economía: venta de productos y compra de animales y piezas de la nave.
- Progresión hasta la reparación de la nave y final con decisión del jugador.
- Interacción en VR: agarrar, soltar y lanzar objetos y animales; locomoción continua con carrera.
- Guardado y carga de partidas en base de datos.
- Sistema de logros.
## Tecnologías
 
| Ámbito | Herramienta |
|---|---|
| Motor | Unity (C#) |
| Realidad virtual | Meta XR SDK, OpenXR, XR Interaction Toolkit |
| Dispositivo objetivo | Meta Quest 3S (standalone) |
| Base de datos | SQLite 3 |
| Control de versiones | Git y GitHub |
| Planificación | Tablero Kanban (GitHub Projects) |
| Audio | LMMS |
 
## Base de datos
 
El modelo se compone de 14 tablas relacionadas entre sí y 2 vistas:
 
- **Jugadores y partidas:** `jugador`, `partida`, `logro`, `logro_jugador`.
- **Catálogos:** `producto`, `tipo_animal`, `tipo_cultivo`, `pieza_nave`.
- **Estado de la granja:** `parcela`, `animal`, `cultivo`, `inventario`.
- **Progresión y economía:** `pieza_comprada`, `transaccion`.
 
## Instalación y ejecución
 
> Pendiente de completar cuando exista una primera versión jugable.
 
1. Instalar Unity (versión indicada en `ProjectSettings/ProjectVersion.txt`) con el módulo de compilación para Android.
2. Clonar el repositorio: `git clone https://github.com/TU_USUARIO/earendel-project.git`
3. Abrir la carpeta del proyecto desde Unity Hub.
4. Conectar un Meta Quest 3S en modo desarrollador y compilar con *Build and Run*.
## Planificación
 
El trabajo se organiza en un tablero Kanban con las fases de preproducción, prototipo VR, sistemas
núcleo, persistencia, progresión y final, contenido, pruebas y entrega.
 
Enlace al tablero: `ENLACE_AL_TABLERO`
 
## Estado actual y próximos pasos
 
- [x] Concepto, música y arte conceptual
- [x] Prototipo VR: locomoción, agarre y lanzamiento
- [ ] IA básica de animales y sistema de comida
- [x] Modelo de base de datos, scripts de creación y datos de prueba
- [ ] Ciclo de cultivo y corral
- [ ] Economía y tienda de piezas de la nave
- [ ] Integración de la base de datos en Unity
- [ ] Final del juego y logros
- [ ] Pruebas en Quest 3S y optimización
## Autor
 
**Iván** — TFG de DAM, curso 2026/2027.
 
## Licencia
 
Pendiente de definir.
 
