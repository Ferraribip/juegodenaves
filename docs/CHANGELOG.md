# Registro de Cambios (Changelog)

Todos los cambios notables en el proyecto **Juego de Naves en Consola (POO C++)** serán documentados en este archivo.

El formato está basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/) y este proyecto adhiere a [Semantic Versioning](https://semver.org/lang/es/).

---

## [1.0.0] - 2026-10-21

### Añadido
- **Clase Nave:** Implementación del jugador con encapsulamiento (`private:` coordenadas $x, y$ y cantidad de $vidas$; `public:` constructores, métodos de movimiento y representación gráfica).
- **Clases Asteroide y Bala:** Modelado de los objetos secundarios del entorno con generación aleatoria y movimiento dinámico.
- **Manejo de Memoria Dinámica:** Uso de `std::vector` de punteros para gestionar colecciones dinámicas de balas y asteroides en tiempo de ejecución.
- **Sistema Anti-Copia / Identificación:** Solicitud inicial del nombre del piloto en consola y renderizado persistente en el HUD durante el juego.
- **Control de Consola (Win32 API):** Integración de `gotoxy()` para posicionamiento de cursor y ocultamiento del puntero de consola con `ocultarCursor()`.
- **Detección de Colisiones:**
  - Colisión Asteroide-Jugador (reducción de vidas y reposicionamiento).
  - Colisión Bala-Asteroide (destrucción de objetos y actualización de pantalla).
- **Documentación Formal:**
  - `README.md` con descripción general, instrucciones de instalación y controles.
  - Informe técnico bajo norma APA v7 en formato PDF.
  - Manual del Programador v1.0.0 y Manual del Usuario v1.0.0.

### Cambiado
- **Refactorización de Arquitectura:** Transición del modelo estructurado en C (`struct`) utilizado en la Actividad 7 hacia la Programación Orientada a Objetos (`class`) con modificadores de acceso.

---

## [0.1.0] - 2026-10-15

### Añadido
- Estructura base del repositorio local (`src/`, `docs/`, `manuales/`, `capturas/`).
- Código fuente prototipo en `src/main.cpp`.
- Configuración de exclusiones en `.gitignore` para archivos de compilación (`.exe`, `.out`, `.vscode/`).
- Archivo de licencia abierta `LICENSE` (MIT).
