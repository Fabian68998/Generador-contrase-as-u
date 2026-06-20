# Generador Seguro de Contraseñas

Este es un proyecto académico de la materia de programación. El sistema genera contraseñas seguras validando la longitud y permitiendo al usuario elegir filtros de seguridad.

## Diagrama de Flujo

```mermaid
graph TD
    A([Inicio]) --> B[/Ingresar longitud de contraseña/]
    B --> C{¿Longitud < 8?}
    C -- Sí --> D[/Mostrar Error/]
    D --> B
    C -- No --> E[/Preguntar por: Mayúsculas, Números, Símbolos/]
    E --> F[Construir lista de caracteres válidos]
    F --> G[Generar contraseña aleatoria iterando con bucle FOR]
    G --> H[/Mostrar contraseña en pantalla/]
    H --> I([Fin])
