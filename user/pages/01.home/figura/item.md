---
title: FIGURA
---

<script type="text/javascript" >


    function recibir() {   
        
     var msj="";
    document.getElementById("nombre").innerHTML =msj;
    var max= document.getElementById("myInput").value;
    //Imprimir figuras de triangulos formados por asteriscos con ciclo for
    var f,c;
    //triangulo rectangulo recto a derechas
    
    for (f=1;f<=max;f++)
    {
        for(c=1;c<=f;c++)
           msj=msj+"*";
        msj=msj+"<br>";
    } 
    //document.write("<br>");
    
    //triangulo rectangulo invertido a izquierdas
    for (f=max-1;f>=1;f--)
    {
        for(c=1;c<=max-f;c++)
            msj=msj+"&nbsp&nbsp";
        for(c=1;c<=f;c++)
            msj=msj+"*";
      msj=msj+"<br>";
    }
    msj=msj+"<br>";
   // document.write("fin");
        document.getElementById("nombre").innerHTML = msj;       

}


/*
        var numero = document.getElementById("texto").value;
        document.getElementById("txt").innerText = numero;
        var n = (numero / 2);

            if (numero % 2 == 0) {
               // document.write("ERROR, Ingrese un numero impar");
               
            }
            else {
                for (var i = 0; i <= n; i++) {
                    for (var j = 0; j < i + 1; j++) {
                        document.write("*");
                    }
                    document.write("<br>");
                }

                for (var i = 1; i <= n; i++) {
                    for (var j = 0; j <= n; j++) {
                        if (j < i) {
                            document.write("&nbsp&nbsp");
                        }
                        else {
                            document.write("*");
                        }
                    }
                    document.write("<br>");
                }
            }
            document.write("<br>");
            document.write("<br>");
        //    document.write('<a href="figura.html">Regresar</a>');
        }


*/
    //}
</script> 


<body>

Ingresa un numero :

<input type="text" id="myInput"  onkeyup="recibir()">
<p id="nombre" style="color:blue;"></p>
<form id="formulario" name="formu">
    	
    	<br>
<!--      Ingresa un numero :
<input type="text" id="texto" onchange="recibir()"/> <!--donde escribe el numero 
-->
<br>
<div id="txt"></div>
</form>
<p id="txt"></p>

</body>


