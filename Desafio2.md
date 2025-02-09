# Resolución del desafío 2

Saber cómo usar funciones es uno de los conceptos fundamentales en la programación y el desarrollo de software. Las funciones desempeñan un papel crucial en la organización, modularización y reutilización del código.

Con eso en mente, hemos creado una lista de actividades (opcionales) centradas en la práctica para mejorar aún más tu experiencia de aprendizaje.



//ACTIVIDAD 1: Crear una función que muestre "¡Hola, mundo!" en la consola.

```javascript
function MensajeSaludo() {
    console.log('¡Hola, mundo!');
} 

MensajeSaludo();
```





//ACTIVIDAD 2: Crear una función que reciba un nombre como parámetro y muestre "¡Hola, [nombre]!" en la consola.

```javascript
function MensajeSaludoNombre(nombre) {
    console.log(`¡Hola, ${nombre}!`);
}

MensajeSaludoNombre('Bibiana');
```






//ACTIVIDAD 3: Crear una función que reciba un número como parámetro y devuelva el doble de ese número.

```javascript
function DuplicarValor(numero) {
    return numero * 2;
}

let ResultadoDuplicar = DuplicarValor(8);

console.log(ResultadoDuplicar);
```






//ACTIVIDAD 4: Crear una función que reciba tres números como parámetros y devuelva su promedio.

```javascript
function Promedio(num1,num2,num3) {
    return (( num1 + num2 + num3 )/3); 
}

let resultadoPromedio = Promedio(2,2,2);
console.log(resultadoPromedio);
```





//ACTIVIDAD 5: Crear una función que reciba dos números como parámetros y devuelva el mayor de ellos.

```javascript
//function numeroMayor(num1,num2) {
//    if(num1>=num2) {
//        return num1;        
//    }else{
//        num2;
//        return num2;
//    }; 
//}



function numeroMayor(num1,num2){
    return num1 > num2 ? num1 : num2 ;
}

let resultadoNumeroMayor = numeroMayor(20,5);
console.log(resultadoNumeroMayor);
```






//ACTIVIDAD 6: Crear una función que reciba un número como parámetro y devuelva el resultado de multiplicar ese número por sí mismo.

```javascript
function Multiplicar(num1) {
    return num1 * 2 ;
}

let resultadoMultiplicar = Multiplicar(8);
console.log(resultadoMultiplicar);
```


