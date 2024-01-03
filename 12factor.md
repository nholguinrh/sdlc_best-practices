#"The Twelve-Factor App" es un conjunto de principios y prácticas que proporcionan pautas para construir aplicaciones modernas, especialmente aquellas que se ejecutan en entornos de nube. Estos principios fueron presentados por Adam Wiggins y Heroku en 2011 y han sido ampliamente adoptados como un marco de referencia para el desarrollo de aplicaciones en la nube. La idea detrás de los "Doce Factores" es ofrecer un enfoque coherente y eficiente para el diseño, desarrollo y operación de aplicaciones, maximizando la portabilidad y escalabilidad.

A continuación, se describen brevemente cada uno de los doce factores:

Codebase: Mantén un solo repositorio de código para una aplicación, pero puedes tener múltiples instancias ejecutándose.

Dependencies: Expresa y aisla las dependencias de la aplicación. Usa un sistema de gestión de dependencias y evita depender de dependencias del sistema operativo.

Config: Almacena la configuración en variables de entorno para separar la configuración del código y facilitar la portabilidad.

Backing services: Trata los servicios externos como recursos adjuntos. Conéctate a servicios, como bases de datos y colas, a través de URLs.

Build, release, run: Separa los procesos de construcción, liberación y ejecución. Esto mejora la reproducibilidad y facilita las actualizaciones.

Processes: Ejecuta la aplicación como uno o más procesos sin estado. Los procesos comparten un espacio de memoria efímero y pueden ser escalados horizontalmente.

Port binding: Exporta servicios a través de la vinculación de puertos. Las aplicaciones deben ser completamente autocontenidas y no confiar en servicios específicos del host.

Concurrency: Escala horizontalmente mediante la adición de procesos. Diseña la aplicación para manejar múltiples instancias que comparten la carga de trabajo.

Disposability: Maximiza la robustez con arranques y apagados rápidos. La aplicación debe ser fácil de iniciar y detener, facilitando el equilibrio de carga y la gestión de fallas.

Dev/prod parity: Mantén la consistencia entre los entornos de desarrollo, prueba y producción. Minimiza las diferencias para evitar sorpresas inesperadas.

Logs: Trata los registros como flujos de eventos. Centraliza los registros y trata los eventos de registro como corrientes de tiempo ordenadas.

Admin processes: Ejecuta tareas administrativas como procesos únicos y puntuales. Estas tareas deben ser manejadas por procesos distintos de los procesos principales de la aplicación.

Adherirse a estos doce factores facilita el desarrollo de aplicaciones que son robustas, escalables, y fácilmente mantenibles, al tiempo que se benefician de las ventajas que ofrece la infraestructura en la nube.
