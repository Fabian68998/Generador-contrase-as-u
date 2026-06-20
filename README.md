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
