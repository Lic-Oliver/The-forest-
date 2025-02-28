# The-forest-
Prueba de repositorio 
document.getElementById('inicioButton').addEventListener('click', function() {
    let usuario = document.getElementById('usuario').value;
    localStorage.setItem('usuario',usuario);//ACA  ESTA  GUARDADO  EL  NOMBRE DEL PERSON

    let password = document.getElementById('password').value;

    let EDAD = document.getElementById('EDAD').value;
    localStorage.setItem('EDAD',EDAD);//ACA GUARDE LA EDAD DEL JUGADOR 

    if (EDAD >= 18 ){
    if(usuario && password) {
        window.location.href = 'inicio.html'
    } else {
        alert('Por favor, completa todos los datos para continuar.');
    }
    }else{
        alert('no tienes edad para jugar');
    }
});
