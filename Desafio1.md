# Resolución del desafío 1

Saber cómo usar funciones es uno de los conceptos fundamentales en la programación y el desarrollo de software. Las funciones desempeñan un papel crucial en la organización, modularización y reutilización del código.

Con eso en mente, hemos creado una lista de actividades (opcionales) centradas en la práctica para mejorar aún más tu experiencia de aprendizaje.


//ACTIVIDAD 2: Cambia el contenido de la etiqueta h1 con document.querySelector y asigna el siguiente texto: "Hora del Desafío".

```javascript
//En el app.js
let titulo = document.querySelector('h1'); // Objeto

titulo.innerHTML = 'Hora del Desafío';   //poner texto al titulo 
```

//ACTIVIDAD 3: Crea una función que muestre en la consola el mensaje "El botón fue clicado" siempre que se presione el botón "Console".

```javascript
//En index.html
 //antes:       <button onclick="" class="button">Console</button>
 //despues:     <button onclick="clickBotonConsola();" class="button">Console</button>

//En el app.js
function clickBotonConsola(){
        console.log('El botón fue clicado');
}
```




//ACTIVIDAD 4: Crea una función que se ejecute cuando se haga clic en el botón "prompt", preguntando el nombre de una ciudad de Brasil. 
// Luego, muestra una alerta con el mensaje concatenando la respuesta con el texto: "Estuve en {ciudad} y me acordé de ti".

```javascript
//En index.html
 //antes:       <button onclick="" class="button">Alert</button>
 //despues:     <button onclick="clickBotonPrompt();" class="button">Alert</button>

//En el app.js
function clickBotonPrompt(){
    let ciudadBrasil = prompt('Ingresa el nombre de una ciudad de Brasil:');
    alert(`Estuve en ${ciudadBrasil} y me acordé de ti`);
}
```


//ACTIVIDAD 5: Crea una función que muestre una alerta con el mensaje: "Yo amo JS" siempre que se presione el botón "Alerta".

```javascript
//En index.html
 //antes:       <button onclick="" class="button">Alert</button>
 //despues:     <button onclick="clickBotonAlerta();" class="button">Alert</button>


//En el app.js
function clickBotonAlerta(){
    alert('Yo amo JS');
}
```



//ACTIVIDAD 6: Al hacer clic en el botón "suma", pide 2 números y muestra el resultado de la suma en una alerta.

```javascript
//En index.html
 //antes:       <button onclick="" class="button">Suma</button>
 //despues:     <button onclick="clickBotonSuma();" class="button">Suma</button>

//En el app.js
function clickBotonSuma(){
        
    let numero1 = parseInt(prompt('Ingresa Valor Número # 1 :')) ;
    let numero2 = parseInt(prompt('Ingresa Valor Número # 2 :')) ; 

    let resultado = numero1 + numero2;
    
    alert(`La suma de ${numero1} + ${numero2} es igual a ${resultado}.`);
}
```
