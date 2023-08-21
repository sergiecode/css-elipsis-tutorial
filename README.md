![Elipsis CSS](https://raw.githubusercontent.com/sergiecode/css-elipsis-tutorial/master/elipsis.jpg)

![Elipsis CSS 2](https://raw.githubusercontent.com/sergiecode/css-elipsis-tutorial/master/elipsis2.png)

# Tutorial de Elipsis en CSS

Este es un tutorial que te guiará a través del proceso de aplicar una elipsis a un texto largo utilizando CSS. Una elipsis es una técnica que muestra solo una parte del contenido de un texto largo y oculta el resto, reemplazándolo con puntos suspensivos. Esto es útil cuando deseas ahorrar espacio en diseño y resaltar solo la parte más importante del contenido.

## Paso 1: Configurar el HTML

Primero, necesitas un documento HTML en el que aplicarás la elipsis al texto. Aquí tienes un ejemplo de cómo podría ser tu estructura HTML:

```
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Tutorial de Elipsis en CSS</title>
</head>
<body>

    <div class="entorno">
        <h1>Aplicar Elipsis</h1>
        <p class="elipsis">En este texto se aplicará la elipsis, ya que es un texto muy largo y no es importante todo el contenido, seguramente se puede ingresar para verlo completo</p>
    </div>
    
</body>
</html>
```

## Paso 2: Estilizar con CSS

Ahora, vamos a aplicar los estilos necesarios utilizando CSS para lograr la elipsis. En este caso, estamos utilizando clases para aplicar estilos específicos al contenido. Asegúrate de tener un archivo `styles.css` en la misma ubicación que tu archivo HTML.


```
/* styles.css */

body {
    background-color: black;
    color: rgb(255, 248, 156);
}

.entorno {
    margin: 300px 50px 0px 50px;
    background-color: rgb(20, 21, 22);
    max-width: 50rem;
}

.elipsis {
    white-space: nowrap; /* Evita el salto de línea */
    overflow: hidden; /* Oculta el contenido sobrante */
    text-overflow: ellipsis; /* Muestra puntos suspensivos al final del contenido truncado */
}
```

## Explicación de los estilos

-   `white-space: nowrap;`: Esto evita que el texto tenga saltos de línea, manteniéndolo en una sola línea.
-   `overflow: hidden;`: Esto oculta cualquier contenido que se desborde del contenedor.
-   `text-overflow: ellipsis;`: Esta propiedad agrega puntos suspensivos al final del contenido cuando se desborda.
