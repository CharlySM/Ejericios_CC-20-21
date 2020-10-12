# Ejercicio 1
## Buscar una aplicación de ejemplo, preferiblemente propia, y deducir qué patrón es el que usa. ¿Qué habría que hacer para evolucionar a un patrón tipo microservicios?

Una aplicación que se hizo en la asignatura tecnologías web de la universidad de Granada. Era una aplicación que gestionaba el login de los usuarios en una página como la principal de la UGR. Donde había distintos tipos de usuarios y cada uno podía acceder a una información distinta.

Esta aplicación tenía una arquitectura por capas, las distintas capas eran: capa de almacenamiento, capa de aplicación y una capa de presentación.

La capa de almacenamiento consta de un gestor de base de datos, que creaba, borraba y actualizaba la información en la base de datos.

La capa de aplicación gestionaba las peticiones entre la capa de presentación y la capa de almacenamiento.

La capa de presentación muestra la recibe las peticiones y muestra la información y cambios que realiza el usuario.

Para convertirlo en una arquitectura de microservicios, se tendría que realizar un microservicio por capa, con un lenguaje que permitiese esto.


# Ejercicio 2
## En la aplicación que se ha usado como ejemplo en el ejercicio anterior, ¿podría usar diferentes lenguajes? ¿Qué almacenes de datos serían los más convenientes?

La aplicación del ejercicio anterior esta desarrollada con PHP, HTML y CSS. Se podría realizar con java, donde un componente se podría dedicar a la capa de la vista y otro componente se podría dedicar a la parte que gestiona las peticiones y cambios que se reciben desde la capa de la vista.  Para la capa de la vista se puede usar lenguaje xhtml. El almacenamiento que se puede usar es Base de datos SQL ya que la base de datos que se usa es relacional por lo que almacenamiento en SQL es ideal, pero se podría usar cualquier base de datos relacional.
