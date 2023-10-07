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

### CSS - Cascading Style Sheets
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
table {
    width: 80%; /*Ancho en toda la pag*/
    background-color: #24283b;
    border-collapse: collapse; /*Quitar borde entre las columnas*/
}

tr:nth-child(even) { /*Seleccionar filas de forma par o impar*/
    /*even => Primera fila; odd => Segunda fila*/
    background-color: #565f89;
}

td {
    border: 1px solid #24283b;
    padding: 8px;
}

table th { /*Cabecera de la tabla*/
    background-color: #0f0f14;
    color: white;
    text-align: left; /*Aliar texto a la izq*/
    padding-left: 8px;
    padding-right: 8px;
    padding-top: 12px;
    padding-bottom: 12px;
}
~~~
Display
~~~
p {
    /*Con esto convertimos en lineas todos*/
    display: inline;
}

span{
    /* con este convertimos en bloques */
    display: block;
}
~~~
Max-width y position
~~~
p {
    max-width: 400px; /*Ancho maximo, no deja hacer scroll*/
    /*width: 500px; /*Ancho maximo pero permite hacer scroll*/
    background-color: #9ece6a;
    margin: auto; /*Margen automatico*/
    /*position: relative; /*Nueva posicion*/
    position: fixed; /*Posicion fija, sirve para los menus estaticos*/
    left: 0px;
    right: 0px;
    top: 0px; /*Corta de arriba hacia abajo*/
    bottom: 690px; /*Corta de abajo hacia arriba*/
}

div {
    color: #9ece6a;
}
~~~
Overflow
~~~
#over {
    width: 100px;
    height: 100px;
    /* overflow: visible;  /*valor por defecto*/
    /*overflow: hidden;  /*corta lo que esta fuera de la caja*/
    /*overflow: scroll; /*Scroll*/
    /*overflow: auto; /*Scroll automatico*/
    /*overflow-y: auto; /*coloca el scroll para el eje vertical*/
    overflow-x: auto; /*coloca el scroll para el eje horizontal */
}
~~~
float, mas selectores y opacidad
~~~
body {
    background-color: #10111c;
    /* color: #9ece6a; */
    color: #aa0505;
    font-size: 30px;
}

img {
    float: right;
}

img:hover { /*PAra resaltar*/
    opacity: 0.9; /*0 trasparente, 1 solido*/
}

div p {
    color: #b97d10;
    font-size: 20px;
}
~~~
Barra de Navegacion
~~~
body {
    background-color: #1a1b26;
    font-size: 18px;
}

ul {
    list-style-type: none; /*eliminar puntos de la lista*/
    margin: 0; /*reiniciar el margen a cero*/
    padding: 0; /*Reiniciar el contenido de la lista*/
    overflow: hidden; 
    position: fixed; /*Posicion fija*/
    top: 0; /*Se queda arriba*/
    left: 0; /*correr hacia la izq*/
    width: 100%; /*El ancho*/
    background-color: #24283b; /*Barra*/
}

li {
    float: left; /*Pega los elementes horizontalmente*/
}

li a {
    display: block;
    color: #9ece6a;
    text-align: center;
    padding: 14px; /*Separacion entre elementos*/
    text-decoration: none;
}

li:hover { /*Sensacion de pasar mouse por encima*/
    background-color: rgba(0, 0, 0, 0.1); /*Trasparencia, la ultima coma es el porcentaje*/
}

.active { /*Color al link inicio*/
    background-color: #565f89;
}

.context {
    margin-top: 60px;
    color: #a9b1d6;
}
~~~
Formularios
~~~
.box {
    background-color: #1a1b26;
    padding: 12px 20px;
    border-radius: 4px;
    box-shadow: 0px 2px 2px rgba(158, 206, 106, 0.1);
}

input[type=text] { /*Así se selecciona todos los input de tipo texto*/
    background-color: #c0caf5;
    width: 100%; /*Ancho de los campos de texgto*/
    padding: 12px 20px;
    margin: 8px 0px;
    display: inline-block;
    border: 1px solid #9ece6a;
    border-radius: 4px;
    box-sizing: border-box;
}

input[type=submit] {
    width: 100%;
    background-color: #9ece6a;
    font-size: 25px;
    color: #1a1b26;
    padding: 14px 20px;
    margin: 8px 0;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

textarea { /*Así se selecciona todos los input de tipo texto*/
    background-color: #c0caf5;
    width: 100%; /*Ancho de los campos de texgto*/
    padding: 12px 20px;
    margin: 8px 0px;
    display: inline-block;
    border: 1px solid #9ece6a;
    border-radius: 4px;
    box-sizing: border-box;
}
~~~
Backgrounds
~~~
.fondo {
    background-color: #565f89;
    height: 500px;
    /*El siguiente es para agregar un relleno de imagen al DIV*/
    background-image: url('https://los40.cl/wp-content/uploads/2021/06/radioformulaqr-768x432.jpg');
    background-repeat: no-repeat; /*Repetir imagen en el DIV*/
    background-position: right bottom; /*Esto mueve la imagen*/
    background-attachment: fixed; /*Scroll para mover la imagen con el texto, fixed para solo mover el texto*/
    background-size: cover; /*Para ajustar la imagen al div*/
}
~~~
Fondos con Gradiente
~~~
.fondo {
    /*Con el "linear-gradient" se puede mezcalr colocres, colocar desde un angulo preciso*/
    /*Se puede usar"to bottom right" o por angulo con deg""*/
    /*Se puede usar mas de un color*/
    background-image:  linear-gradient(to bottom right, red, blue);
    /*Para colocar como si fuera un barrilete*/
    background-image: repeating-linear-gradient(to bottom right, red, blue, 20%, green 30%);
}
~~~
Sombras
~~~
.box {
    /*cuando se agrega el inset el elemento esta hundido, sin este es como si flotara*/
    box-shadow: 0px 1px 2px rgba(158, 206, 106, 0.5) inset;
}
.box2 {
    box-shadow: 0px 1px 2px rgba(158, 206, 106, 0.5);
}

.text {
    color: #1a1b26;
    font-size: 30px ;
    /* Esto es para darle sombra al texto */
    text-shadow: 0px 1px 4px rgba(158, 206, 106, 0.8);
}
~~~
Trasformaciones en 2D y 3D
~~~
.box {
    position: relative;
    left: 50px;
    top: 50px;
    width: 150px;
    height: 100px;
    background-color: #565f89;
    box-shadow: 1px 2px 2px rgb(180, 249, 248, 0.8);
    transform: rotate(20deg); /*Girar 20grados */
    transform: translate(50px, 10px); /*Trasladar*/
    transform: scale(1.05, 1.05); /*Escalar*/
    transform: skewX(-10deg); /*Retorcer*/
    /*Trasformaciones en 3D*/
    transform: rotateX(20deg); /*Este rota con el eje X y Y*/
}
~~~
Transiciones animadas
~~~
.box {
    position: relative;
    left: 50px;
    top: 50px;
    width: 150px;
    height: 100px;
    background-color: #565f89;
    box-shadow: 1px 2px 2px rgb(180, 249, 248, 0.8);
    /* transition: width 0.3s; */
    transition: 0.3s; /*Este tiempo es el tiempo que demora hacer la transicion*/
    transition-delay: 0.5s; /*Delay en la animacion*/
    /*Otra forma de hacer la transicion y el delay en una sola linea*/
    /* transition: 0.3s 0.5s; */
}

.box:hover {
    /* width: 200px; */
    transform: scale(1.05,1.05);
    background-color: #1a1b26;
}
~~~
Ejercicios de Cajas
~~~
body {
    background-color: #565f89;
    color: #cfc9c2;
}

.box {
    background-color: #1a1b26;
    box-shadow: 0px 2px 2px rgb(180, 249, 248, 0.8);
    margin: 10px 15px; /*Separacion entre cajas*/
    width: 200px; /*Ancho maximo*/
    padding: 10px 15px; /*expande margen vertical horizontal*/
    text-align: center;
} 

.red {
    border-left: 2px solid red;
}

.red:hover {
    transform: scale(1.05, 1.05);
}

.green {
    border-left: 2px solid green;
}

.green:hover {
    box-shadow: 0px 2px 8px rgb(180, 249, 248, 0.8);
}

.blue {
    border-left: 2px solid blue;
}

.blue:hover {
    background-color: #414868;
}
~~~
### CSS Grid
 es una propiedad CSS que se utiliza para crear un contenedor que sigue el modelo de diseño de cuadrícula (grid layout). Con esta propiedad, puedes organizar elementos en filas y columnas en una cuadrícula, lo que te brinda un alto grado de control sobre el diseño de tu página web.
~~~
body {
    background-color: #1a1b26;
    color: #ff9e64;
}

.grid {
    display: grid; /*Activar todo como grilla, todo lo que contenga ese elemento */
    display: inline-grid; /*En vez de usar todo el ancho, solo usa el espacio en sus elementos*/
}

.element {
    background-color: #24283b;
    padding: 10px 15px;
}
~~~
Columnas y filas
~~~
.grid {
    display: grid; /*Activar todo como grilla, todo lo que contenga ese elemento */
    grid-template-rows: 50px 50px 50px; /*Esto define los px de las filas, aca solo se definieron 3 los demas quedan por defecto*/
    /*grid-template-columns: 100px 50px 50px; /*Define tamaño de Col*/
    grid-template-columns: 1fr 2fr 3fr; /*Este utiliza la fracciones de la pagina*/
    /*Tambine se puede usar combinado como "2rem 20% 1fr 2fr"*/
}
~~~
Tamaño Minimo y Maximo
~~~
.grid {
    display: grid;
    grid-template-rows: minmax(100px, auto);
    grid-template-columns: minmax(auto, 50%) 1fr 2fr;
}

.element {
    background-color: #24283b;
    padding: 10px 15px;
}
~~~
