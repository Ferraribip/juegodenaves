🎮🚀 Juego de Naves en Consola — POO en C++Proyecto correspondiente a la Actividad N° 8 de la asignatura Laboratorio de Programación (LPR). Implementación de un juego de naves arcade en consola de comandos utilizando el paradigma de Programación Orientada a Objetos (POO) en C++.📋 Información InstitucionalInstitución: E.E.S.T. N° 1 "Eduardo Ader" — Vicente LópezCurso: 5° Año 3° División (Grupos A-B)Materia: Laboratorio de Programación (LPR)Profesor: Mansilla Muñoz York Elías (@docentedeclasesdeapoyo)Ciclo Lectivo: 2026 — 2° Cuatrimestre🎯 Objetivos de AprendizajeEvolución del Paradigma: Transición formal desde Estructuras (struct) hacia Clases (class).Diseño de Clases & Encapsulamiento: Definición explícita de miembros privados (private:) y públicos (public:), garantizando la integridad de datos como la posición, vida y límites de las entidades.Manejo de Memoria y Punteros: Uso dinámico de objetos en memoria mediante std::vector de punteros para asteroides y proyectiles (Bala*, Asteroide*).Documentación Profesional de Software: Generación del informe bajo la norma APA v7 junto a los manuales de usuario y del programador.🕹️ Características del Juego y ControlesEl juego consiste en pilotar una nave espacial dentro de una grilla delimitada en la consola, esquivando e impactando asteroides mediante disparos.ControlesTeclaAcciónWMover hacia arribaSMover hacia abajoAMover hacia la izquierdaDMover hacia la derechaESPACIODisparar proyectil📂 Estructura del RepositorioEl proyecto cumple estrictamente con la estructura formal requerida para la entrega e integración en GitHub / GitLab:juegodenaves/
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
🛠️ Requisitos e InstalaciónRequisitos PreviosOS: Windows (debido a las librerías de consola <windows.h> y <conio.h>).Compilador: GCC / MinGW (g++) habilitado en la variable de entorno PATH, o IDEs como Code::Blocks / Visual Studio Code.Compilación y EjecuciónClonar el repositorio:git clone https://github.com/TU_USUARIO/juegodenaves.git
cd juegodenaves
Compilar el código fuente:g++ -o juegodenaves.exe src/main.cpp
Ejecutar el simulador:./juegodenaves.exe
🧬 Conceptos Técnicos AplicadosEncapsulamiento (private vs public): Ocultamiento de coordenadas (x, y) y del estado interno (vidas) para prevenir manipulaciones indebidas desde el main().Constructores: Inicialización parametrizada de las propiedades de las entidades al momento de instanciarlas (Nave, Asteroide, Bala).Métodos Getters: Puertas de acceso controlado (getX(), getY(), getVidas()) para lectura segura de atributos.Control de Consola (Win32 API): Posicionamiento con SetConsoleCursorPosition mediante la función gotoxy(x, y) e invisibilidad del cursor con CONSOLE_CURSOR_INFO.📄 LicenciaEste proyecto se distribuye bajo la licencia MIT. Para más detalles, consulte el archivo LICENSE.
