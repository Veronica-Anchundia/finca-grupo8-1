# TALLER 1: Consolidación de la Poo en Java 21 y Entorno Profesional

Proyecto Maven del **Taller 1: Configuración del entorno profesional** (Programación 3, POO avanzada). Deja funcionando, en equipo, el entorno de trabajo con **Java 21, IntelliJ IDEA, Maven, JUnit 5 y Git/GitHub**.
## 1 Información del Grupo
| | |
|---|---|
| **Universidad** | Universidad Agraria del Ecuador, Facultad de Ciencias Agrarias "Dr. Jacobo Bucaram Ortiz" |
| **Carrera** | Computación en Línea |
| **Grupo** | 08 · Cuarto semestre, paralelo C |
| **Asignatura** | Programación 3 (POO) |
| **Período** | 2026-2027 CII |
| **Docente** | Ing. Hamilton Francisco Villamar Barros, MSc. |

## 2 Integrantes y roles

| Integrante | Rol en el taller | Usuario de GitHub |
|---|---|---|
| María Anchundia | Líder de integración | [vero11-lang](https://github.com/vero11-lang) |
| Narciso Galarza | Responsable de pruebas | [galarzanarciso-lab](https://github.com/galarzanarciso-lab) |
| Brithany Rivera | Responsable de pruebas | [brithanyrivera1502-hue](https://github.com/brithanyrivera1502-hue) |
| Alfonso Olvera | Responsable de documentación | [gansudokentpc-oss](https://github.com/gansudokentpc-oss) |
| Michael Caicedo | Verificador | [Michael1994-link](https://github.com/Michael1994-link) |
 
 ## 3. Objetivo
Configurar en equipo el entorno profesional de desarrollo de la asignatura JDK21, IntelliJ IDEA, Maven, JUnit 5 y Git con GitHub y demostrarlo con un proyecto Maven compartido, con pruebas unitarias aprobadas y un historial de commits en el que participen todos los integrantes.


## Versiones utilizadas

| Integrante | Java (Temurin) | Git | IntelliJ IDEA |
|---|---|---|---|
| María Anchundia | 21.0.3 | 2.52.0 | 2025.3.1 |
| Narciso Galarza | 21 y 25.0.3 (usa el 21 para el taller) | 2.52.0 | 2025.3.1 |
| Brithany Rivera | 21.0.7 | 2.52.0 | 2025.3.1 |
| Alfonso Olvera | 21.0.3 | 2.52.0 | 2025.3.1 |
| Michael Caicedo | 21.0.3 | 2.52.0 | 2025.3.1 |

## Estructura del proyecto

```
finca-grupo08
├── pom.xml
├── .gitignore
├── README.md
└── src
    ├── main/java/ec/edu/uagraria/finca/Parcela.java
    └── test/java/ec/edu/uagraria/finca/
        ├── ParcelaTest.java
        └── Parcela<Apellido>Test.java   (una por integrante)
```

- **GroupId:** `ec.edu.uagraria.prog3`
- **Dependencia de pruebas:** JUnit 5 (Jupiter) 5.10.2
- **Compilación:** Java 21 (`maven.compiler.release`)

## Cómo ejecutar las pruebas

1. Clonar el repositorio:
   ```
   git clone https://github.com/galarzanarciso-lab/finca-grupo8.git
   cd finca-grupo8
   ```
2. Verificar las versiones instaladas:
   ```
   java -version
   git --version
   ```
   La primera línea de `java -version` debe comenzar con `openjdk version "21`.
3. Abrir el proyecto en IntelliJ IDEA con el JDK 21.
4. En la ventana **Maven**, abrir **Lifecycle** y hacer doble clic en **test**, o ejecutar:
   ```
   mvn test
   ```
5. El resultado esperado termina en:
   ```
   Tests run: N, Failures: 0, Errors: 0, Skipped: 0
   BUILD SUCCESS
   ```
   La primera vez Maven descarga bibliotecas y puede tardar; no cancelar el proceso.

## Flujo de trabajo en equipo

Cada integrante agrega su propia clase de prueba (un archivo por persona para evitar conflictos) y la publica desde su cuenta:

```
git add .
git commit -m "Agrega prueba de <Apellido>"
git pull --rebase
git push
```

## Honestidad académica

Cada integrante realiza sus propios commits desde su propia cuenta de GitHub. El uso de asistentes de inteligencia artificial se declara en el informe del taller.
