# Proyecto de Simulación de Vehículo en Three.js

## Descripción General
Este proyecto es una simulación interactiva en 3D desarrollada con Three.js, donde un vehículo controlado por el usuario puede moverse, disparar proyectiles y destruir obstáculos. La escena incluye iluminación dinámica, texturas detalladas y elementos interactivos como una barra de cooldown y un contador de obstáculos restantes.

---

## Cambios y Mejoras en la Nueva Versión

### 1. Movimiento Dinámico de la Luz
Se añadió un efecto de animación para la luz direccional. La posición de la luz cambia dinámicamente en la escena, simulando una fuente de luz en movimiento que ilumina los objetos desde diferentes ángulos. Esto puede aportar mayor realismo y dinamismo visual.

**Nueva función:**  
- `animateDirectionalLight()`

---

### 2. Implementación de Mapas de Normales
Se mejoraron los obstáculos introduciendo texturas con mapas de normales. Esto permite que la iluminación interactúe con la superficie de los 2 nuevos objetos creados de forma más realista, resaltando detalles tridimensionales en las texturas.

**Nuevas funciones relacionadas:**  
- `createObstacleWithNormals(x, y, z)`
- `createSphereWithNormals(x, y, z)`

---

### 3. Overlays Gráficos
Se añadieron dos elementos gráficos superpuestos que enriquecen la experiencia del usuario:
- **Barra de Cooldown:** Indica cuándo el cañón está listo para disparar nuevamente. Esta barra se llena gradualmente después de cada disparo y cambia de color dependiendo de su estado.
- **Contador de Obstáculos:** Muestra el número de obstáculos restantes en la escena, actualizándose dinámicamente a medida que el jugador los destruye.

**Nuevas funciones relacionadas:**  
- `updateCooldownBar(progress)`
- `updateObstacleCounterText(count)`

---
