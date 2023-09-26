<p align="center">
  <a target="blank"><img src="https://persis.es/wp-content/uploads/2021/07/HTML5-CSS3-1.png" alt="Javascript Logo @clipartmax.com" width="200" /></a>
</p>
<p align="center">
  <strong><span style="font-size: 30px;">HTML Y CSS</span></strong>
</p>

## HTML
La etiquieta **head** no va a mostrar nada.
PAra mostrar contenido se usa la etiqueta de **body**
PAra colocar un titulo se usa la etiqueta **title** este se vera reflejado en la pestaña.
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JefersonRomero</title>
</head>
<body>
    <h1>Titulo 1</h1>
    <h2>Titulo 2</h2>
    <h3>Titulo 3</h3>
    <h4>Titulo 4</h4>
    <h5>Titulo 5</h5>
    <h6>Titulo 6</h6>
    <p>Hola! esto es un parrafo!</p>
    <hr />    
    <p>Hola! <br />esto es un salto de linea</p> <!-- Cuando la etiqueta no tiene contenido, se usa esta forma para cerrarla <br /> -->
    <p>Este es mi <b>Parrafo 3!</b></p> <!-- Negrita <b> -->
    <blockquote>Esta es una cita!</blockquote> <!-- forma de citar -->
    <code>Esto es codigo<br /></code> <!-- Esto es para colocar codigo   -->
    <em>Texto con enfasis<br /></em> <!-- Esto es para colocar enfasis   -->
    <i>Otra forma de colocar texto con enfasis o italic cursiva<br /></i>
    <pre>Preformateado<br /></pre>
    <s>Preformateado<br /></s>
    <small>Texto pequeño<br /></small>
    <strong>Texto en negrita<br /></strong>
    <u>Texto subrayado<br /></u>
    <div>Sección 1!</div> <!-- Son Secciones diferents y da el salto de linea de una  --> 
    <div>Sección 2!</div>
    <div>Sección 3!</div>
</body>
</html>
~~~
### Formularios e Inputs
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formularios</title>
</head>
<body>
    <fieldset> <!--Agrupa las etiquetas en uno solo-->
        <legend>Credenciales</legend> <!--Nombra la agrupacion de campos-->
        <form action=""> <!--Para crear formulario, el action dirije a la ruta el boton de guardar, por defecto es al servidor-->
        <label for="">Nombre</label>
        <input type="text" placeholder="Nombre..."><br /> <!--Texto dentro del input-->
        <label for="">Telefono</label>
        <input type="number"><br />
        <label for="">password</label>
        <input type="password"><br />
        <input type="submit"><br /> <!-- Enviar info del formulario -->
        <input type="submit" value="Enviar =)"><br /> <!-- Enviar info del formulario -->
        <textarea name="" id="" cols="30" rows="10"></textarea> <!-- Ingresar parrafos de texto  -->
        <button>Aceptar</button> <!-- otra forma de crear botones -->
        <select name="" id="">
            <option value="goku">Goku</option><!-- el valor que se vera es Goku, en mayuscula, pero el que se vera en codigo es goku en minuscula -->
            <option value="vegeta">Vegeta</option>
            <option value="brolly">Brolly</option>
        </select>
        </form>
    </fieldset>
</body>
</html>
~~~
### Imagenes y Links
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Listas Ordenadas y No Ordenadas</title>
</head>
<body>
    
</body>
</html>
~~~
### Listas Ordenadas y no Ordenadas
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Listas Ordenadas y No Ordenadas</title>
</head>
<body>
    <ul> <!--Lista NO Ordenada-->
        <li> Elemento 1</li> <!--Elementos de la lista-->
        <li> Elemento 2</li>
        <li> Elemento 3</li>
    </ul>
    <ol> <!--Lista Ordenada-->
        <li> Elemento 1</li>
        <li> Elemento 2</li>
        <li> Elemento 3</li>
    </ol>
</body>
</html>
~~~
### Tablas, Cabeceras, pie, filas y celdas
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>tcpfc</title>
</head>
<body>
    <table>
        <thead>
            <tr> <!--Filas-->
                <th>Mes</th>
                <th>Ahorros</th> <!--Cabecera-->
            </tr>
        </thead> <!--Columnas-->
        <tbody> <!--contenido-->
            <tr>
                <td>Enero</td>
                <td>$1.000</td>
            </tr>
            <td>Febrero</td>
            <td>$500</td>
        </tbody>
        <tfoot> <!--Pie de la talba-->
            <tr>
                <td>Suma Total:</td>
                <td>$1.500</td>
            </tr>
        </tfoot>
    </table>
</body>
</html>
~~~

## CSS - Cascading Style Sheets
Tenemos el Siguiete HTML
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS</title>
    <link rel="stylesheet" href="main.css" type="text/css">
</head>
<body>
    <p>Hola Mundo!</p>
    <p id="parrafo">Este es un párrafo</p>
    <span class="etiqueta">Este es un span</span>
    <br />
    <span class="etiqueta">Este es un segundo span</span>
    <br />
    <span class="etiqueta">Este es un tercer span</span>
</body>
</html>
~~~
Y asignamos el siguiete CSS a este
~~~

body {
    background-color: #efefef;
    color: #7800AC /* Color por defecto de las letras del body*/
}

#parrafo {
    color: #ff0000;
}

.etiqueta {
    color:#00aa00;
}
~~~
Cuando se crea un div así en el HTML
~~~
<body>
    <div class="caja">Hola Mundo!</div>
</body>
~~~
Y esta es su configuracion en CC
~~~z

body {
    background-color: #efefef;
}

.caja {
    margin: 8px; /*Permite separar la margen del body hacia la Der*/
    padding: 8px; /*Permite tomar el contenido y enviarlo mas hacia el centro*/
    border-style: solid; /*Tipo de linea de la caja*/
    border-width: 8px; /*ancho de la linea de la caja*/
    border-color: #faa; /*Color del borde de la caja*/
    border-left: 6px solid #afa; /*Para reemplazar el de la izq*/
    /*top=arriba; bottom=abajo; right=Der*/
    background-color: #aaf; /*Color de fondo*/
    border-radius: 8px; /*curvatura en las cajas, suavizado*/
    height: 20px; /*Alto de la caja*/
    width: 100px; /*Ancho de la caja*/
    color:#ffffff; /*Color de texto*/
}
~~~
Modificaciones de Links en CSS
~~~
p {
    font-family: "Verdana"; /*Tipo de letra*/
    font-weight: 100; /*Negrita*/
    font-style: italic; /*Cursividad o estilo de letra*/
    font-size: 20px; /*Tamaño de letra*/
    color: #222fff;
    text-align: justify;
    text-indent: 15px;/*Identar*/
    line-height: 1.7; /*Con esto validamos el interlineado*/
    word-spacing: 10px; /*Espacio entre las palabras*/
    text-shadow: 1px 2px 2px rgba(0, 0, 0, 0.3); /*Este crea una sombra, el primero lo mueve en x, el segundo en y y el tercero es el nivel de opacidad*/

}

a {
    text-decoration: overline; /*Para colocar el subrayado encima del texto*/
    text-decoration: line-through; /*Para colocar el subrayado en medio del texto*/
    text-decoration: underline; /*Para colocar el subrayado en la parte de abajo del texto*/
    text-decoration: none; /*Para quitar Subrayado*/
    
    text-transform: lowercase; /* Cambiar a minuscula*/
    text-transform: uppercase; /* Cambiar a mayuscula*/
    text-transform: capitalize; /* Cambiar la primera letra a Mayuscula*/

    letter-spacing: 3px; /*Separacion entre letras*/
}
~~~
Parte 2
~~~
a {
    color: #2ac3de;
    font-size: 50px;
    font-family: fantasy;
    padding: 5px;
    border-radius: 4px;
}

a:link {
    color: #9ece6a; /*Este color es cuando no ha sido visitado*/
    text-decoration: none;
}
a:visited{
    color: #2ac3de; /*Cuando ha sido visitado*/
}
a:hover {
    color: #b4f9f8; /*Cuando se pasa el mouse por encima*/
    text-decoration: underline;
    background-color: #25262b;
}
a:active {
    color: #ff9e64; /*Cuando damos click*/
}
~~~
Listas
~~~
body {
    background-color: #1a1b26;
    color: #9ece6a;
    font-size: 30px;
}

/* ul li { Forma de seleccionar al hijo */
    /* list-style-type: lower-greek; Forma simbolo de la lista no ordenada */
    /*Puede ser circle, square, upper-roman, lower-alpha, lower-greek*/
/* } */

ul { /*Padre*/
    list-style-type: none;
    background-color: #414868;
    border: solid 1px #9aa5ce;
    border-radius: 5px;
    padding-left: 0px;
}

li { /*Hijo*/
    border-bottom: solid 1px #9aa5ce;
    padding: 10px;
}
~~~
Tablas
~~~

~~~
