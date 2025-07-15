# sugar-cli: Control de Glucosa CLI Multilenguaje y Multiplataforma

## Índice
* [Acerca del Proyecto](#acerca-del-proyecto)
* [Objetivo General](#objetivo-general)
* [Características Transversales](#características-transversales)
* [Lenguajes y Herramientas](#lenguajes-y-herramientas)
* [Etapas del Desarrollo](#etapas-del-desarrollo)
* [Contribuir](#contribuir)
* [Licencia](#licencia)

## Acerca del Proyecto
"sugar-cli" es un proyecto ambicioso para desarrollar una aplicación de línea de comandos versátil para el control de registros de glucosa. Se diferencia por su enfoque multilenguaje y multiplataforma, explorando las fortalezas de varios lenguajes de programación en el desarrollo de una herramienta única.

## Objetivo General
Desarrollar una aplicación de línea de comandos para convertir y gestionar registros de glucosa, progresando en complejidad y en siete lenguajes (C++, Python, Java, C#, Go, Rust, F#).

## Características Transversales
* Repositorio contenedor con submódulos (uno por lenguaje) y gestión por **tags** (`etapa-<n>-<clave>`).
* Integración de **TDD** desde la etapa 0.
* Flujo ligero inspirado en **12‑Factor App**.
* CI intermedio con **GitHub Actions**.
* Entorno Linux (Debian WSL, Ubuntu ARM, Arch macOS).
* Sin contenedores hasta la etapa 8; Docker/Podman y scripts nativos a partir de la 9.

## Lenguajes y Herramientas
| Lenguaje | TDD        | CLI flags         | UI texto     | Gráficas CLI      | Config global |
| -------- | ---------- | ----------------- | ------------ | ----------------- | ------------- |
| C++      | GoogleTest | CLI11             | ncurses      | ncurses‑plot      | TOML          |
| Python   | pytest     | argparse          | Blessed      | termplotlib       | TOML          |
| Java     | JUnit 5    | picocli           | Lanterna     | —                 | TOML          |
| C#       | xUnit      | CommandLineParser | gui.cs       | gui.cs gráficos   | TOML          |
| Go       | go test    | cobra             | termui       | termui charts     | TOML          |
| Rust     | cargo test | clap              | ncurses      | plotters + tui-rs | TOML          |
| F#       | Expecto    | Argu              | Terminal.Gui | gui.cs gráficos   | TOML          |

## Etapas del Desarrollo
Este proyecto se desarrollará en 30 etapas, comenzando con la configuración del repositorio y avanzando progresivamente en funcionalidades y complejidad. Cada etapa se implementará de forma independiente en cada lenguaje.

*   **Etapa 0:** Preparación del repositorio
*   **Etapa 1:** Casting básico
*   ... (Lista completa de etapas en la descripción del proyecto)

## Contribuir
Las contribuciones son bienvenidas. Por favor, lee las [Directrices de Contribución](CONTRIBUTING.md) (un archivo que crearemos más adelante) para más detalles.

## Licencia
Este proyecto está licenciado bajo la Licencia MIT - consulta el archivo [LICENSE](LICENSE) para más detalles.