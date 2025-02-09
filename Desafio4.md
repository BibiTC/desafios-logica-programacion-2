# Resolución del desafío 4

Saber cómo usar funciones es uno de los conceptos fundamentales en la programación y el desarrollo de software. Las funciones desempeñan un papel crucial en la organización, modularización y reutilización del código.

Con eso en mente, hemos creado una lista de actividades (opcionales) centradas en la práctica para mejorar aún más tu experiencia de aprendizaje.

//Lógica de programación: explorar funciones y listas `
//04. Listas
//DESAFIO: Hora de Practicar


//ACTIVIDAD 1: Crea una lista vacía llamada "listaGenerica".

```javascript
let listaGenerica = [];
```

//ACTIVIDAD 2: Crea una lista de lenguajes de programación llamada "lenguagesDeProgramacion con los siguientes elementos: 'JavaScript', 'C', 'C++', 'Kotlin' y 'Python'.

```javascript
let lenguajesDeProgramacion = ['JavaScript', 'C', 'C++', 'Kotlin' , 'Python'];
```

//ACTIVIDAD 3: Agrega a la lista "lenguajesDeProgramacion los siguientes elementos: 'Java', 'Ruby' y 'GoLang'.

```javascript
lenguajesDeProgramacion.push('Java', 'Ruby' , 'GoLang');
```

//ACTIVIDAD 4: Crea una función que muestre en la consola todos los elementos de la lista "lenguagesDeProgramacion.

```javascript
function mostrarElementosListaAscendente(){
    for (let i = 0; i < lenguajesDeProgramacion.length ; i++) {
        console.log(lenguajesDeProgramacion[i]);
    }
}

mostrarElementosListaAscendente();
```

//ACTIVIDAD 5: Crea una función que muestre en la consola todos los elementos de la lista "lenguagesDeProgramacion en orden inverso.

```javascript
function mostrarElementosListaDescendente(){
    for (let i = lenguajesDeProgramacion.length-1 ; i >= 0 ; i--) {
        console.log(lenguajesDeProgramacion[i]);
    }
}

mostrarElementosListaDescendente();
```

//ACTIVIDAD 6: Crea una función que calcule el promedio de los elementos en una lista de números.


```javascript
let listaNumeros = [5,10,15,20,25,30];
let resultado = 0;
let promedio = 0;

function calculoPromedioNumerosLista(listaNumeros){
    console.log(listaNumeros.length);
    for (let i = 0; i < listaNumeros.length; i++) {
        console.log(`i : ${i}`);
        //console.log(Typeof(listaNumeros(i)));
        console.log(`${listaNumeros[i]}`);
        resultado = resultado + listaNumeros[i]; // resultado += listaNumeros[i];
    }
    console.log(`Resultado ${resultado}, Longitud Array ${listaNumeros.length} `);
    promedioNumeros = resultado / listaNumeros.length;
    return promedioNumeros;
}
    
promedio = calculoPromedioNumerosLista(listaNumeros);
console.log(`Promedio : ${promedio}`);
```

//==================================================================================================
//ACTIVIDAD 7: Crna función que muestre en la consola el número más grande y el número más pequeño en una lista.

```javascript
let listaNum = [2,8,10,50,90,80,1];
let maximo = listaNum[0];
let minimo = listaNum[0];

function MostrarMaximoMinimo(listaNum){
    for (let i = 0; i < listaNum.length; i++) {
        if(listaNum[i] > maximo){
            maximo = listaNum[i];
        } else if(listaNum[i] < minimo){
            minimo = listaNum[i]   
        } 
    }
    console.log(`Max : ${maximo} `);
    console.log(`Min : ${minimo} `);
    return;
}

MostrarMaximoMinimo(listaNum);
```


//======================================================================================================
//ACTIVIDAD 8: Crea una función que devuelva la suma de todos los elementos en una lista.


```javascript
function sumarLista(listaNumerosSumar) {
    let resultadoSuma = 0;
    for (let i = 0; i < listaNumerosSumar.length; i++) {
        resultadoSuma += listaNumerosSumar[i];
    }
    return resultadoSuma;
}

let listaNumerosSumar = [20,30,40,50,1,10,9];
let Suma = sumarLista(listaNumerosSumar); 
console.log(`Resultado Sumar Numeros de Array: ${Suma}`);

//ACTIVIDAD 9: Crea una función que devuelva la posición en la lista donde se encuentra un elemento pasado como parámetro, o -1 si no existe en la lista.


function buscarElemento(lista,buscarElemento) {
    for (let i = 0; i < lista.length; i++) {
        if (lista[i] == buscarElemento){
            return i; // Encontro el elemento
        }
    }
    return -1; // No encontro el elemento
}

let lista = [2,8,50,10,60,40];
let valorbuscar = 40;
let resultadoBusqueda = buscarElemento(lista,valorbuscar);
console.log(`El elemento ${valorbuscar}, ${resultadoBusqueda == -1 ? 'no existe en la lista': 'existe en la lista'}`);
```
   
//ACTIVIDAD 10: Crea una función que reciba dos listas de números del mismo tamaño y devuelva una nueva lista con la suma de los elementos uno a uno.

```javascript
function sumaListas(lista1,lista2) {
    
    let SumaDosArray = lista1.map((item, ix) => item + lista2[ix]);
    return SumaDosArray;
    }
    
let lista1 = [2,8,50,10,60,40];
let lista2 = [1,9,60,20,70,50];
let operacionSumaListas = sumaListas(lista1,lista2);
console.log(operacionSumaListas);
```

//ACTIVIDAD 11: Crea una función que reciba una lista de números y devuelva una nueva lista con el cuadrado de cada número.

```javascript
function cuadradoListas(lista) {
    
    let ListaCuadrado = lista.map((item, ix) => Math.pow(lista[ix],2));
    return ListaCuadrado;
    }
    
let lista = [2,8,50,10,60,40];
let operacionCuadradoLista = cuadradoListas(lista);
console.log(operacionCuadradoLista);
```

 