## Javascript

[Cos'è la Coercion in JavaScript? (Entry)]()

[Qual è la funzione dell'operatore typeof? (Junior)]()

[Cos'è il tipo di dato oggetto? (Junior)]()

[Spiegazione degli array in JavaScript. (Junior)]()

[Spiegazione dell'uguaglianza in JavaScript? (Junior)]()

[Cos'è lo Scope in JavaScript? (Junior)]()

[Qual è la funzione della keyword "let" in JavaScript? (Mid)]()

[Spiegazione di un Callback con un semplice esempio. (Mid)]()

[Cos'è la Strict Mode? (Mid)]()

[Qual è la funzione di "use strict"? (Mid)]()

[Cos'è un Polyfill? (Mid)]()

[Come verificare che un numero sia intero? (Mid)]()

[Spiegazione dei tipi di dato in JavaScript. (Mid)]()

[Posto di avere un array non ordinato contenente (n - 1) di n numeri consecutivi (avendo definito i limiti) trovare il numero mancante mantenendo un tempo di esecuzione di O(n). (Mid)]()

[Rimuovere gli elementi duplicati di un array e ritornare un nuovo array con gli elementi rimasti. (Mid)]()

[Data una stringa, invertire il verso di ogni parola. (Mid)]()

[Scrivere una funzione che ti permetta di fare questo. (Mid)]()

[Implementare l'accodamento(enqueue) e l'estrazione(dequeue) di un elemento usando solamente due stacks. (Mid)]()

[Come usare una closure per creare un contatore private. (Mid)]()

[Spiegazione di Null e Undefined in JavaScript. (Sesior)]()

[Spiegazione dell'Event Bubbling e del modo per impedirlo. (Mig)]()

[Come verificare che un oggetto sia un array? (Mid)]()

[Scrivere una "mul" function. (Mid)]()

[Come svuotare un array in JavaScript? (Mid)]()

[Come confrontare due oggetti in JavaScript? (Mid)]()

[Dato un array di interi, trovare la più grande differenza tra due elementi in modo tale che l'elemento più piccolo venga sempre prima dell'elemento più grande. (Senior)]()

[Trovare l'intersezione tra due array. L'intersezione sarebbe l'elemento comune presente in entrambi gli array. In questo caso l'elemento è uno solo. (Senior)]()

[Scrivere una funzione che ti permetta di fare questo. (Senior)]()

[Date due stringhe, ritornare True se esiste un anagramma tra loro. (Senior)]()

[Verificare se una stringa data è un palindromo. Attenzione alla Case Sensitivity. (Senior)]()

[Qual è la differenza tra un Shim e un Polyfill? (Senior)]()

[Quale sarà l'output del seguente blocco di codice? (Senior)]()

[Sai spiegare la differenza tra ES5 ed ES6? (Senior)]()

[Cos'è un'IIFE (Immediately Invoked Function Expressions)? (Senior)]()

[Quale sarà l'output del seguente blocco di codice? (Senior)]()

[Quale sarà l'output del seguente blocco di codice? (Senior)]()

[Fornisci alcuni esempi di Coercion tra un valore non booleano ad uno booleano. (Senior)]()

[Spiega la differenza tra Undefined e Not Defined in JavaScript. (Senior)]()

[Quale sarà l'output del seguente blocco di codice? (Senior)]()

[What is the drawback of creating true private in JavaScript? (Senior)]()

[Qual è la differenza tra una funzione ed una funzione anonima? (Senior)]()

[Dato un array di interi, trovare il prodotto più grande prodotto da tre degli interi dati. (Senior)]()

[Descrivi il concetto di Clousure in JavaScript come meglio riesci. (Senior)]()

[Scrivi una funzione ricorsiva che ritorna la stringa binaria di un dato numero decimale. (Senior)]()

[Cos'è una Clousure in JavaScript? Fornisci un esempio. (Expert)]()

[Spiegazione del concetto di Hoisting in Javascript. (Expert)]()

[Dato un intero, determinare se è una potenza di 2. In tal caso, ritornare il suddetto numero, altrimenti -1. (Expert)]()

[Quale sarà l'output del seguente blocco di codice? (Expert)]()

[Descrivere il Module Design Pattern in JavaScript. (Expert)]()

[Come creare una variabile privata in Javascript? (Expert)]()

[Descrivere il Prototype Design Pattern in JavaScript. (Expert)]()

[Scrivere una funzione ricorsiva in grado di eseguire una ricerca binaria. (Expert)]()

[Creare una funzione in grado di valutare se una data espressione ha parentesi bilanciate usando le stack. (Expert)]()

[Quale sarà l'output del seguente blocco di codice? (Expert)]()

[Spiegazione dell'ereditarietà con la catena di prototipi in JavaScript. (Expert)]()

[A cosa fa riferimento il termine Transpiling in JavaScript? (Expert)]()

[Qual è la funzione della keyword "new" in JavaScript? (Expert)]()

[Quando si utilizza la funzione Bind in JavaScript? (Expert)]()

[Qual è il concetto alla base della keyword "this"? Fornire alcuni esempi. (Expert)]()

[Come inserire il proprio metodo all'oggetto array per permettere al seguente blocco di codice di funzionare? (Expert)]()

[Cos'è l'Hoisting in JavaScript? (Expert)]()

[Quale sarà l'output del seguente blocco di codice? (Expert)]()

[Veriricare se la stringa data è isomorfica. (Expert)]()

[Descrivere il Revealing Design Pattern in JavaScript. (Expert)]()



### Cos'è la Coercion in JavaScript? (Entry)

In JavaScript la conversione tra due tipi di dato primitivi è chiamata `coercion`. La coercion può essere applicata in due casi: *esplicita* ed *implicita*.

Di seguito un esempio della *coercion* esplicita:
```js
var a = "42";

var b = Number(a);

a;      // "42"
b;      // 42 -- il numero
```
Qui invece un esempio della *coercion* implicita:
```js
var a = "42";

var b = a * 1; // coercion implicita che porta il valore a 42

a;      // "42"
b;      // 42 -- il numero
```



[[↑] Back to top](#JavaScript)
### Qual è la funzione dell'operatore typeof? (Junior)

JavaScript mette a disposizione l'operatore `typeOf`, il quale esamina il valore dato e ritorna il tipo di dato.
```js
var a;
typof(a);       // "undefined"

a = "hello world";
typeof a;      // "string"

a = 42;
typeof a;      // number

a = true
typeof a;      // boolean

a = null
typeof a;      // "object" --gotcha

a = undefined
typeof a;      // "undefined"

a = { b: "c" };
typeof a;      // "object"
```



[[↑] Back to top](#JavaScript)
### Cos'è il tipo di dato oggetto? (Junior)

Il tipo di dato oggetto si riferisce ad un valore composto al quale è possibile impostare delle proprietà, le quali mantengono a loro volta il loro tipo di dato.
```js
var obj = {
    a: "hello world", // proprietà
    b: 42,
    c: true
};

obj.a;      // "hello world" -- accesso con dot notation
obj.b;      // 42
obj.c;      // true

obj["a"];   // "hello world" -- accesso con la bracket notation
obj["b"];   // 42
obj["c"];   // true
```

La *brcket notation* è utile se si vuole accedere alla proprietà ma il nome risiede in un'altra variabile, come nel segunte esempio:
```js
var obj = {
    a: "hello world",
    b: 42
};

var b = "a";

obj[b];     // "hello world"
obj["b"];   // 42    
```



[[↑] Back to top](#JavaScript)
### Spiegazione degli array in JavaScript. (Junior)

Un `array` è un oggetto che contiene valori di qualsiasi tipo che non fanno riferimento ad un nome o ad una proprietà, ma ad una specifica posizione:
```js
var arr = [
    "hello world",
    42,
    true
];

arr[0];         // "hello world"
arr[1];         // 42
arr[2];         // true
arr.length;	    // 3

typeof arr;     // "object"
```



[[↑] Back to top](#JavaScript)
### Spiegazione dell'uguaglianza in JavaScript? (Junior)

Javascript mette a disposizione due tipologia di confronto, una di tipo strict ed una di tipo type-converting:
* **Strictg comparsion (e.g. ===)** verfica l'uguaglianza dei valori senza permettere la *coercion*
* **Abstract comparsion (e.g. ==)** verifica l'uguaglianza dei valori permettendo la *coercion*

```js
var a = "42";
var b = 42;

a == b;     // true
a === b;    // false
```
Alcune regole di uguaglianza:
* Se uno dei due valori potrebbe risultare un valore `true` oppure `false`, utilizzare `===` anzichè `==`.
* Se uno dei due valori rientra tra uno dei seguenti tipi di valore, `0`, `""` oppure `[] (array vuoto)` allore utilizzare `===` anzichè `==`.
* In tutti gli altri casi, sarai al sicuro utilizzando `===`. Non solo è maggiormente sicuro, ma in molti casi semplificherà il tuo codice miglirando la leggibilità.



[[↑] Back to top](#JavaScript)
### Cos'è lo Scope in JavaScript? (Junior)

In JavaScript ogni funzine ha il proprio *scope*. Lo *scope* essenzialmente è una raccolta di variabili e relative regole di accesso alle suddette variabili. Solo il codice inserito all'interno della funzione può accedere alla variabili in *scope*

I nomi delle variabili devono essere univoci. Lo *scope* può essere annidato all'interno di un altro *scope*. Se uno *scope* è annidato all'interno di un altro, il codice presente all'interno del più annidato può accedere alle variabili da entrambi gli *scope*.



[[↑] Back to top](#JavaScript)
### Qual è la funzione della keyword "let" in JavaScript? (Mid)

Oltre a permettere la dichiarazione di varibili a livello di funzione, ES6 ti permette di dichiarare variabili appartenenti al blocco individuale utilizzando la keyword `let`.

###### Fonte

* https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md



[[↑] Back to top](#JavaScript)
### Spiegazione di un Callback con un semplice esempio. (Mid)

Un `callback` è una funzione passata come parametro di un'altra funzione come argomento, eseguita solo al termine di altre determinate operazioni. Di seguito un esempio di un callback che logga a console solo al termine di alcune operazioni.
```js
function modifyArray(arr, callback) {
    // modifico lo stato dell'array
    arr.push(100);
    // eseguo il collback passato come argomento
    callback()
}

var arr = [1, 2, 3, 4, 5];

modifyArray(arr, function() {
    console.log("l'array è stato modificato", arr);
});
```

###### Fonte

* https://coderbyte.com/algorithm/10-common-javascript-interview-questions



[[↑] Back to top](#JavaScript)
### Cos'è la Strict Mode? (Mid)

La *Strict mode* è una funzionalità aggiunta in ECMAScript 5 che permette di inserire un programma od una funzione all'interno di un contesto con determinate restrizioni. Questo cosiddetto contesto *strict* previene l'esecuzione di possibili operazioni indesiderate e genera un numero maggiore di eccezioni.
```js
// modalità non-strict

(function() {
    "use strict";

    // definisco la libreria con restrizioni
})();

// modalità non-strict
```



[[↑] Back to top](#JavaScript)
### Qual è la funzione di "use strict"? (Mid)

L'espressione `use strict` è posizionata all'inizio di un file .js oppure all'inizio di una funzione. Questa aiuta a scrivere codice maggiormente sicuro lanciando un'eccezione se una variabile globale è stata create per errore. Per esempio, il seguente blocco di codice lancerà un'eccezione:
```js
function doSomething(val) {
    "use strict";
    x = val + 10;
}
```

Lancerà un'eccezione perchè `x` non è stata definita ed è stata settata nello *scope* globale. Questa operazione non è consentita nella modalità strict. Per rimediare procedere come segue:

```js
function doSomething(val) {
    "use strict";
    var x = val + 10
}
```

###### Fonte

* https://coderbyte.com/algorithm/10-common-javascript-interview-questions



[[↑] Back to top](#JavaScript)
Cos'è un Polyfill? (Mid)

*Polyfill* fa riferimento a dello specifico codice (o plugin) che ti permette di avere delle specifiche funzionalità in browser che non implementano di default la suddetta funzionalità.

###### Source

* http://www.programmerinterview.com/index.php/html5/html5-polyfill/



[[↑] Back to top](#JavaScript)
### Come verificare che un numero sia intero? (Mid)

Un semplice metodo per verificare se un dato numero è un intero è dividendolo per 1 e constatando se il risultato presenta un resto.
```js
function isInt(num) {
    return num % 1 === 0;
}

console.log(isInt(4));      // true
console.log(isInt(12.2));   // false
console.log(isInt(0.3));    // false
```

###### Source

* https://coderbyte.com/algorithm/10-common-javascript-interview-questions