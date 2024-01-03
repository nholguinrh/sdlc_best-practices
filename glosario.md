Glosario:

I. Código base (Codebase):
El código base es cualquier repositorio (en un sistema de control de versiones centralizado como Subversion), o cualquier conjunto de repositorios que comparten un commit raíz (en un sistema de control de versiones descentralizado como Git).
El código base de la aplicación es único.
El código base es el mismo en todos los despliegues, aunque pueden ser diferentes versiones en cada despliegue.

II. Dependencias:
Declara todas sus dependencias, completamente y explícitamente, mediante un manifiesto de declaración de dependencias. Además, usa herramientas de aislamiento de dependencias durante la ejecución para asegurar que las dependencias, implícitamente, no afectan al resto del sistema.

III. Configuración:
La configuración de una aplicación es todo lo que puede variar entre despliegues (entornos de preproducción, producción, desarrollo, etc).

IV. Backing services:
Un backing service es cualquier recurso que la aplicación puede consumir a través de la red como parte de su funcionamiento habitual. Entre otros ejemplos, podemos encontrar bases de datos, los sistemas de mensajería y de colas, los servicios SMTP de email, y los sistemas de cache.

V. Construir, distribuir, ejecutar:
Las aplicaciones hacen una separación completa de las fases de construcción, de distribución y de ejecución. Por ejemplo, es imposible hacer cambios en el código en la fase de ejecución, porque no hay una manera de propagar dichos cambios a la fase de construcción.

VI. Procesos:
La aplicación se ejecuta como uno o más procesos en el entorno de ejecución sin estado.

VII. Asignación de puertos:
Las aplicaciones son completamente auto-contenidas y no dependen de un servidor web en ejecución para crear un servicio web público. 

VIII. Concurrencia:
Los procesos de las aplicaciones se inspiran en el modelo de procesos de unix para ejecutar demonios. Usando este modelo, el desarrollador puede distribuir la ejecución de su aplicación para gestionar diversas cargas de trabajo asignando cada tipo de trabajo a un tipo de proceso (worker).

IX. Desechabilidad:
Los procesos de las aplicaciones son desechables, lo que significa que pueden iniciarse o finalizarse en el momento que sea necesario. 

X. Igualdad entre desarrollo y producción:
Las aplicaciones están diseñadas para hacer despliegues continuos que reducen las diferencias entre los entornos de desarrollo y producción.

XI. logs:
Existen medios que permiten observar el comportamiento de la aplicación durante su ejecución.

XII. Administración de procesos:
Ejecutar las tareas de gestión/administración como procesos que solo se ejecutan una vez.
