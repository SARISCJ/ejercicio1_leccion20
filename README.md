# ejercicio1_leccion20

INICIO

var num2 = 0;

function suma(num1) {
	return function() {
		return num1 + num2;
	}
} 

var suma2 = suma(2);
console.log(suma2(5)); // Debería mostrar 7 de resultado

var suma12 = suma(12);
console.log(suma12(76)) // Debería mostrar 88 de resultado.

FIN

var num2 = 0;

function suma(num1) {
	return function(num2) {
		return num1 + num2;
	}
} 

var suma2 = suma(2);
console.log(suma2(5)); // Debería mostrar 7 de resultado

var suma12 = suma(12);
console.log(suma12(76)) // Debería mostrar 88 de resultado.

Modifique la linea :
		return function(num2)
 por que el parametro num2 es una variable global y por eso se puede llamar dentro de una funcion.  

