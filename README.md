# InicioDeSesion
<meta charset="UTF-8">
<br>
<h1>Solo es un juego</h1>
<h2></h2>

<br>
<script>

    function saltarlinea() {
        document.write("<br>");
        document.write("<br>");
        document.write("<br>");
    }


    function imprimir(frase) {

        document.write(frase)
        saltarlinea()

    }


    function saltarLinea() {
        document.write("<br>");    
        document.write("<br>");    
        document.write("<br>");    
    }  

    function imprimir(frase) {
        document.write(frase);
        saltarLinea();
    } 

   
    var inicioDeSesionRegistrado = "alura";
    var contrasenhaRegistrada = "alura321";
    var maximoIntentos = 3
    var intentoActual = 1

    while(intentoActual <= maximoIntentos) {

    var inicioDeSesionIngresado = prompt("Ingrese su usuario");
    var contrasenhaIngresada = prompt("Ingrese su contraseña");

    if(inicioDeSesionRegistrado == inicioDeSesionIngresado && contrasenhaRegistrada == contrasenhaIngresada ) {
        alert("Bienvenido al sistema " + inicioDeSesionIngresado);
        intentoActual = maximoIntentos
    } 
    else {
        if(intentoActual == 3){
            alert("Agotaste el número permitido de intentos!")}
            else{
                alert("Inicio de sesion invalido, por favor inente de nuevo")
            }
    }
    intentoActual = intentoActual +1
}
</script>
