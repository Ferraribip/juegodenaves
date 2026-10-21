# 🎮🚀 Juego de Naves en Consola — POO en C++

[![C++](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)](https://isocpp.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Institution](https://img.shields.io/badge/E.E.S.T.-N%C2%B01%20Eduardo%20Ader-red.svg)](#)
[![Subject](https://img.shields.io/badge/Materia-Laboratorio%20de%20Programaci%C3%B3n-green.svg)](#)

Proyecto correspondiente a la **Actividad N° 8** de la asignatura **Laboratorio de Programación (LPR)**. Implementación de un juego de naves arcade en consola de comandos utilizando el paradigma de **Programación Orientada a Objetos (POO)** en C++.

---

## 📋 Información Institucional

* **Institución:** E.E.S.T. N° 1 "Eduardo Ader" — Vicente López
* **Curso:** 5° Año 3° División (Grupos A-B)
* **Materia:** Laboratorio de Programación (LPR)
* **Profesor:** Mansilla Muñoz York Elías (`@docentedeclasesdeapoyo`)
* **Ciclo Lectivo:** 2026 — 2° Cuatrimestre

---

## 🎯 Objetivos de Aprendizaje

1. **Evolución del Paradigma:** Transición formal desde Estructuras (`struct`) hacia Clases (`class`).
2. **Diseño de Clases & Encapsulamiento:** Definición explícita de miembros privados (`private:`) y públicos (`public:`), garantizando la integridad de datos como la posición, vida y límites de las entidades.
3. **Manejo de Memoria y Punteros:** Uso dinámico de objetos en memoria mediante `std::vector` de punteros para asteroides y proyectiles (`Bala*`, `Asteroide*`).
4. **Documentación Profesional de Software:** Generación del informe bajo la norma APA v7 junto a los manuales de usuario y del programador.

---

## 🕹️ Características del Juego y Controles

El juego consiste en pilotar una nave espacial dentro de una grilla delimitada en la consola, esquivando e impactando asteroides mediante disparos.

### Controles
| Tecla | Acción |
| :---: | :--- |
| <kbd>W</kbd> | Mover hacia arriba |
| <kbd>S</kbd> | Mover hacia abajo |
| <kbd>A</kbd> | Mover hacia la izquierda |
| <kbd>D</kbd> | Mover hacia la derecha |
| <kbd>ESPACIO</kbd> | Disparar proyectil |

---

## 📂 Estructura del Repositorio

El proyecto cumple estrictamente con la estructura formal requerida para la entrega e integración en GitHub / GitLab:

```text
juegodenaves/
├── .gitignore                  # Filtros de compilación (.exe, .out, .vscode/)
├── LICENSE                     # Licencia Abierta MIT
├── README.md                   # Presentación principal del proyecto
├── CHANGELOG.md                # Registro de cambios y versionado
├── docs/
│   └── InformeEEST1_LPR2026_ACT08_v1.0.0.pdf   # Informe formal en formato APA v7
├── manuales/
│   ├── manual_programador_v1.0.0.pdf          # Documentación técnica
│   └── manual_usuario_v1.0.0.pdf              # Guía de uso e instalación
├── src/
│   └── main.cpp                # Código fuente principal en C++
└── capturas/
    └── combate_consola.png     # Captura de pantalla con HUD e identificación
```

---

## 🛠️ Requisitos e Instalación

### Requisitos Previos
* **OS:** Windows (debido a las librerías de consola `<windows.h>` y `<conio.h>`).
* **Compilador:** GCC / MinGW (g++) habilitado en la variable de entorno PATH, o IDEs como Code::Blocks / Visual Studio Code.

### Compilación y Ejecución
1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/TU_USUARIO/juegodenaves.git
   cd juegodenaves
   ```
2. **Compilar el código fuente:**
   ```bash
   g++ -o juegodenaves.exe src/main.cpp
   ```
3. **Ejecutar el simulador:**
   ```bash
   ./juegodenaves.exe
   ```

---

## 🧬 Conceptos Técnicos Aplicados

* **Encapsulamiento (`private` vs `public`):** Ocultamiento de coordenadas (`x`, `y`) y del estado interno (`vidas`) para prevenir manipulaciones indebidas desde el `main()`.
* **Constructores:** Inicialización parametrizada de las propiedades de las entidades al momento de instanciarlas (`Nave`, `Asteroide`, `Bala`).
* **Métodos Getters:** Puertas de acceso controlado (`getX()`, `getY()`, `getVidas()`) para lectura segura de atributos.
* **Control de Consola (Win32 API):** Posicionamiento con `SetConsoleCursorPosition` mediante la función `gotoxy(x, y)` e invisibilidad del cursor con `CONSOLE_CURSOR_INFO`.

---

## 📄 Licencia

Este proyecto se distribuye bajo la licencia **MIT**. Para más detalles, consulte el archivo [LICENSE](LICENSE).