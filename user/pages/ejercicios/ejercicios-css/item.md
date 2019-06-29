---
title: 'EJERCICIOS CSS '
published: true
visible: true
---

<!-- # BIENVENIDOS
## Graficación y animación  -->

###EJERCICIOS CSS
EJERCICIO 1 -> BACKGROUND

/*1. Colores de fondo en todo el body*/
/*2. Colores de fondo en todo los p*/
/*3. Poner un gif en todo el body*/ 
/*4. Poner la imagen en el boy de forma horizontal y si queremos le cambiamos a y que es vertical */ 
/*5. Colores de fondo en todo los p*/ 
/*6. Poner un gif en todo el body*/ 
/*7. Poner la imagen en el boy de forma horizontal y si queremos le cambiamos a y que es vertical */

1. 
body {
background-color:#FAF0E6 
}
2. 
p {background-color:#F55FDA }
3. 
body{
background-image: url(.gif);
}    
4.
body {
background-image: url("data:image.jpg");
background-repeat: repeat-x;
}  

5.

body {
background-color:#FAF0E6  /*colores de fondo en todo el body*/
}
p{background-color:#F55FDA 
}
6. 
body{
background-image: url(.gif);
}    
7. 
body {
background-image: url("data:image/jpeg}


/* EJERCICIO 2 -> BODER*/

/*1. Permite poner cuadros alrededor de p> con un ancho de 3px. en border-style puede haber dotted, solid, ridge, dotted solid,inset. se puede escoger cualquiera*/ 
/*2. Linea 2px color verde */


1.
p {
border-style: dashed;
border-width: 3px;
}  

2.   
p {
border: 2px solid green;
} 
    


/* EJERCICIO 3 -> MARGIN*/

/*1. Permite poner h1 resaltado con azul con margen izquierdo 60px */ 
/*2. Permite poner h1 resaltado con azul y el margen de 25px */ 
/*3. Permite poner h1 resaltado con azul y margen superior y inferior 50px y margen izquierdo y derecho 25px */ 
/*4. Permite tener a h1 en el centro con el margin: auto */


1.
h1 {
background-color: lightblue;
margin-left: 60px;
} 

2.
h1 {
background-color: lightblue;
margin: 25px;
} 

3.
h1 {
background-color: lightblue;
margin: 50px 25px;
} 

4.
h1 {
background-color: lightblue;
width: 300px;
margin: auto;
} 


/* EJERCICIO 4 -> PADDING*/

/*1. Relleno superior de p a "30px" */ 
/*2. Relleno completo a en p con 50px */ 
/*3. Permite poner h1 resaltado con azul y relleno superior y inferior 50px y relleno izquierdo y derecho 25px */


1.
p {
background-color: lightblue;
padding-top: 30px;
} 

2.
p {
background-color: lightblue;
padding: 50px;
} 

3.
p {
background-color: lightblue;
padding: 50px 50px;
} 

/* EJERCICIO 5 -> height-width*/
/*1. Altura 100px y anchura 50% */


h1 {
background-color: lightblue;
height: 100px;
width:50% 
} 


/* EJERCICIO 6 -> Box Model*/

/*1. Modelo de caja nos permite poner azul con ancho de 200px y relleno de 25px */

div {
background-color: lightblue;
width: 200px;
padding: 25px;
}


/* EJERCICIO 7 -> Outline*/

/*1. Contorno "sólido", "5px" para p> y ese solido con un ancho de 5px y que sea color verde*/ 
/*2. Contorno punteado(dotted) color rojo y 10 px */

1.
p {
outline-style: solid;
outline-width: 5px;
outline-color: green;
}

2.
p {
outline: red dotted 10px;
} 


/* EJERCICIO 8 -> Text CSS*/

/*1. Todo el body color rojo y h1 a azules */ /*2. Aliniar al centro h1 */ /*3. Quitar el subrayado de a */

1.  
body {
color: red;
}


h1 {
color: blue;
} 

2.
h1 {
text-align: center;
} 

3.
a {
text-decoration: none;
} 


/* EJERCICIO 9 -> CSS Font*/

/*1. Tipo de letra "Courier New"*/
/*2. Los elementos de p como texto "cursiva". */

1.
body {
font-family: "Courier New";
} 

2. 
p {
font-style: italic;
}


/* EJERCICIO 10 -> CSS LINKS*/

a:link {
text-decoration: none;
}

/* visited link */
a:visited {
text-decoration: none;
}

/* mouse over link */
a:hover {
text-decoration: underline;
}

/* selected link */
a:active {
text-decoration: underline;
}

/*enlaces no visitados en "rojo" y el color de los enlaces visitados "azul" */


/* unvisited link */
a:link {
color: red;
} /* enlace no visitado  */

/* visited link */
a:visited {
color: green;
} /* enlace visitado */

/* mouse over link */
a:hover {
color: hotpink;
} /* mouse enlace selecionado se vuelve azul */

/* selected link */
a:active {
color: blue;
} /* mouse enlace selecionado se vuelve azul */


/* EJERCICIO 11 -> CSS LISTS*/

/*1. Permite cambiar la viñeta puede ser square, circle, lower-alpha, upper-roman*/ 
/*2. Eliminar viñeta */
1.
ul {
list-style-type: square;
} 
ol {
list-style-type: upper-roman;
}

2.
ul {
list-style-type: none;
} 

/* EJERCICIO 12 -> CSS TABLE*/

/*1. Nos permite realizar una tabla de color verde y con doble borde*/
/*2. Hacer una tabla normal de color negro con un 1px aplicando a td y th */
/*3. Tabla de color negro de forma solid aplicando a td y th pero td alineado a lado derecho */


1.
table, th, td {
border: 2px solid green;
} 

table {
border-collapse: collapse;
}

2.
table, td, th {
border: 1px solid black;
} 

3.
table, td, th {
border: 1px solid black;
}
td {
text-align: right;
} 

/* EJERCICIO 13 -> CSS POSITIONING */


/*1. Nos permite poner la una imagen encima de lo que esta escrito */

1.
    img {
    position: absolute;
    left: 0px;
    top: 0px;
    } 

/* EJERCICIO 15 -> CSS ALIGN*/
/*1. Centrar alinea el elemento div> usando márgenes. */
/*2. Coloque el elemento div> completamente a la derecha utilizando el posicionamiento absoluto con position y right*/


1.
div {
    margin-left: auto;
    margin-right: auto;
    width: 300px;
    background-color: #b0e0e6;
}

2.
div {
    position: absolute;
    right: 0px;
    width: 300px;
    background-color: #b0e0e6;
}  
/* EJERCICIO 16 -> CSS COMBINATORS*/ 
/*1. Cambie el color de todos los elementos p>, que son descendientes de los elementos div>, a "rojo*/ 
/*2. Cambie el color de todos los elementos p>, que son hijos inmediatos de los elementos div>, a "rojo". */

1.
div p {
    color: red;
}

2.
div > p {
    color: red;
}  

/* EJERCICIO 17 -> CSS PSEUDO-CLASESS*/


/* unvisited link */
a:link {
background-color: lightblue;
}

/* visited link */
a:visited {
background-color: lightblue;
}

/* mouse over link */
a:hover {
background-color: yellow;
}

/* selected link */
a:active {
background-color: yellow;
} /*1. Cambiar el color del fondo de azul a amarrillo*/



2.
p:first-child {
background-color: lightblue;
}/*2. El color de fondo de los elementos 
, que son el primer elemento secundario de cualquier elemento, en "lightblue".*/




/* EJERCICIO -> CSS COLOR */


/*1. Nos permite poner la una imagen encima de lo que esta escrito */
/*1. Poner la opacidad del color de fondo del elemento h1> en "0.3" utilizando un color RGBA en lugar de RGB.*/
/*2. Establezca el tono en rojo (0), la saturación en 100% y la luminosidad en 50%.*/

1.
h1 {
background-color: rgb(0,255,0);
}  

2.
h1 {
background-color: hsl(0,100%,50%);
}   
/* EJERCICIO -> CSS GRADIENTS */
/*1. Poner un fondo de degradado lineal para el elemento div>, de arriba a abajo, pasando de "blanco" a "verde".*/
/*2. Poner un fondo de degradado lineal para el elemento div>, desde la parte superior izquierda a la parte inferior derecha, pasando de "blanco" a "verde".*/



1.
div {
background-image: linear-gradient(white, green);
} 
2.
div {
background-image: linear-gradient(to bottom right, white, green);
}

/* EJERCICIO -> CSS SHOW EFFECTS */
/*1. Una sombra de texto horizontal de "2px" y vertical de "2px" para el elemento h1>.*/
/*2. Cambie el color de la sombra del texto a "verde" y establezca un radio de desenfoque de "5px". */




1.
h1 {
text-shadow: 2px 2px;
} 
2.
h1 {
text-shadow: 2px 2px 5px green;
} 
/* EJERCICIO -> CSS TEXT
/*1. Permite especificar que el contenido desbordado para el elemento

se debe señalar con puntos suspensivos (...)*/ */
/*2. El elemento

debe ajustarse, incluso si necesita dividirse en medio de una palabra. Con word-wrap: break-word realizamos esto*/

1.
p {
white-space: nowrap; 
width: 200px; 
border: 1px solid #000000;
overflow: hidden;
text-overflow: ellipsis;
} 

2.
p {
width: 150px; 
border: 1px solid #000000;
word-wrap: break-word;
}  
/* EJERCICIO -> CSS WEB FONTS */

1.
@font-face {
font-family: sansation;
src: url(sansation_light.woff);
}

body {
font-family: sansation;
}  /*1. Una fuente web con el nombre "sansation" y la URL "sansation_light.woff".*/

2.
@font-face {
font-family: sansation;
src: url(sansation_light.woff);
}

@font-face {
font-family: sansation;
src: url(sansation_bold.woff);
font-weight: bold;
}

body {
font-family: sansation;
}
/*  Agregue otra regla @ font-face para los caracteres en negrita de la fuente "sansation". Utilice la URL "sansation_bold.woff"
*/ 
/* EJERCICIO -> CSS 2D TRANSFORMS */ /*el elemento

100px a la derecha y 200px hacia abajo. utilizando el transform: translate(100px,200px) */ /*2. Gire el elemento
45 grados. En transform rotate a 45deg*/

1.
div {
width: 100px;
height: 100px;
background-color: lightblue;
border: 1px solid black;
transform: translate(100px,200px);
}
2.
div {
width: 100px;
height: 100px;
margin: 50px;
background-color: lightblue;
border: 1px solid black;
transform: rotate(45deg);
}


/* EJERCICIO -> CSS 3D TRANSFORMS */ /*1. Gira el elemento div en 150 grados en el eje x*/ /*2. Gire el elemento div> 120 grados alrededor de su eje Y. */

1.
div {
width: 100px;
height: 100px;
background-color: lightblue;
border: 1px solid black;
transform: rotateX(150deg);
} 

2.
div {
width: 100px;
height: 100px;
background-color: lightblue;
border: 1px solid black;
transform: rotateY(120deg);
} 


/* EJERCICIO -> CSS TRANSITIONS */ /*1. La transicion del elemento tiene una curva de velocidad al poner el mouse */ 
/*2. Un efecto de transicion de 2 segundos permitiendo girar el cuadrado y cambiandolo de color a azul*/

1.
div {
width: 100px;
height: 100px;
background: red;
transition: width 2s;
transition-timing-function: ease-in-out;
}

div:hover {
width: 300px;
} 

2.
div {
width: 100px;
height: 100px;
background: red;
transition: background 2s, transform 2s;
}

div:hover {
background: blue;
transform: rotate(180deg);
}  


/* EJERCICIO -> CSS ANIMATIONS */
/*1. Nos permite cambiar el cuadrado de color rojo a verde en dos segundos*/
/*2. Nos permite cambiar de color en la posicion izquierda a "0px", la posición superior a: "0px" este con color rojo. La posición izquierda a "0px", la posición superior a: "200px" de color azul. Luego la posición izquierda en "200px", la posición superior en: "200px" de color verde. La posición izquierda a "200px", posición superior a: "0px" de color amarrillo y luego regresa a su posicion inicial con color rojo. */

1.
div {
width: 100px;
height: 100px;
background-color: red;
animation-name: example;
animation-duration: 2s;
}

@keyframes example {
from {background-color: red;}
to {background-color: green;}
}
2.
div {
width: 100px;
height: 100px;
position: relative;
background-color: red;
animation-name: example;
animation-duration: 4s;
}

@keyframes example {
0%   {background-color: red; left:0px; top:0px;}
25%  {background-color: blue; left:0px; top:200px;}
50%  {background-color: green; left:200px; top:200px;}
75%  {background-color: yellow; left:200px; top:0px;}
100% {background-color: red; left:0px; top:0px;}
} 


3.
div{
width: 100px;
height: 100px;
position: relative;
background-color: red;
animation-name: example;
animation-duration: 2s;
animation-delay: 1s;
}

@keyframes example {
0%   {background-color: red; left:0px;}
50%  {background-color: blue; left:200px;}
100% {background-color: red; left:0px;}
} /* La animacion tiene un segundo de retraso al comenzar y va cambiando de rojo a azul. */

