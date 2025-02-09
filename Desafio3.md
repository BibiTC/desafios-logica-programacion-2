//Lógica de programación: explorar funciones y listas `
//03. Reiniciando el Juego
//DESAFIO: Hora de Practicar



//ACTIVIDAD 1: Crea una función que calcule el índice de masa corporal (IMC) de una persona a partir de su 
// altura en metros y peso en kilogramos, que se recibirán como parámetros.

```javascript
function IndiceMasaCorporal(estaturaMetros,pesoKilogramos){
    let imc = pesoKilogramos / (estaturaMetros * estaturaMetros);
    return imc;
}

//Ejemplo :
let imc2 = IndiceMasaCorporal(1.72,60);
console.log(imc2);
```




//ACTIVIDAD 2: Crea una función que calcule el valor del factorial de un número pasado como parámetro.
```javascript
function CalculoFactorial(numero){
    let factorial = numero;
    let resultado = numero;
 
    if (numero == 0 || numero == 1) {
        return 1 ;
    } else {
        while ( factorial > 1 ) { 
            resultado = resultado * (factorial -1)
            factorial--;
           }
           return resultado;
    }
}

// Ejemplo 
let valor = 5
let FactorialEjecucion = CalculoFactorial(valor);
console.log(`El factorial de ${valor} es ${FactorialEjecucion}`);
```

//ACTIVIDAD 3: Crea una función que convierta un valor en dólares, pasado como parámetro, y devuelva el valor 
// equivalente en reales(moneda brasileña,si deseas puedes hacerlo con el valor del dólar en tu país). 
// Para esto, considera la cotización del dólar igual a R$4,80.


```javascript
function CambioDolaresPesos(montoDolares) {
    let tasaDeCambio = 4800;
    let valorPesos = montoDolares * tasaDeCambio;
    return valorPesos;
}

// Ejemplo:
let  dolares = 100;
let  pesos = CambioDolaresPesos(dolares);
console.log(`${dolares} dolares en COP$ ${pesos}`);
```

//ACTIVIDAD 4: Crea una función que muestre en pantalla el área y el perímetro de una sala rectangular, 
// utilizando la altura y la anchura que se proporcionarán como parámetros.

```javascript
function CalcularAreaPerimetroRectangulo(alto,ancho) {
    let Area = alto * ancho;
    let Perimetro = (alto + ancho) * 2;
    return; 
}

// Ejemplo:
let  altoRectangulo = 10;
let  anchoRectangulo = 20;
let calculo = CalcularAreaPerimetroRectangulo(altoRectangulo,anchoRectangulo);
console.log(calculo);
//Pregunto en Grupo
 ```


//ACTIVIDAD 5: Crea una función que muestre en pantalla el área y el perímetro de una sala circular, 
// utilizando su radio que se proporcionará como parámetro. Considera Pi = 3,14.

```javascript
function CalcularAreaPerimetroCirculo(radio) {
    let Pi = 3.14;
    let Area = Pi * (radio * radio) ;
    let Perimetro = 2 * Pi * radio;
    console.log(`Area : ${Area} , Perimetro: ${Perimetro}`)
    return; 
}

// Ejemplo:
let  radio = 10;
let calculocirculo = CalcularAreaPerimetroCirculo(radio);
console.log(`Area : ${CalcularAreaPerimetroCirculo(radio)} , Perimetro: ${CalcularAreaPerimetroCirculo(radio)}`)
```




//ACTIVIDAD 6: Crea una función que muestre en pantalla la tabla de multiplicar de un número dado como parámetro.

```javascript
function tablaDeMultiplicar(numero) {
    
    for (let i = 1; i <= 10; i++) {
        let resultado = numero * i;
        console.log(`${numero} X ${i} = ${resultado}`);
    }
    return ;
}

// Ejemplo:
let  numeroTabla = 10;
tablaDeMultiplicar(numeroTabla);
```

