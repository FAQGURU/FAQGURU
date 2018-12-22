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

[Rimuovere gli elementi duplicati da un array e restituire un nuovo array con gli elementi restanti. (Mid)]()

[Data una stringa, invertire il verso di ogni parola. (Mid)]()

[Scrivere una funzione che ti permetta di fare questo. (Mid)]()

[Implementare l'accodamento(enqueue) e l'estrazione(dequeue) di un elemento usando solamente due stack. (Mid)]()

[Come usare una closure per creare un contatore di tipo private. (Mid)]()

[Spiegazione di Null e Undefined in JavaScript. (Senior)]()

[Spiegazione dell'Event Bubbling e del metodo per impedirlo. (Mid)]()

[Come verificare che un oggetto sia un array? (Mid)]()

[Scrivere una "mul" function. (Mid)]()

[Come svuotare un array in JavaScript? (Mid)]()

[Come confrontare due oggetti in JavaScript? (Mid)]()

[Dato un array di interi, trovare la più grande differenza tra due elementi in modo tale che l'elemento più piccolo venga sempre prima dell'elemento più grande. (Senior)]()

[Trovare l'intersezione tra due array. L'intersezione sarebbe l'elemento comune presente in entrambi gli array. In questo caso l'elemento è uno solo. (Senior)]()

[Scrivere una funzione che ti permetta di fare questo. (Senior)]()

[Date due stringhe, restituire True se esiste un anagramma tra loro. (Senior)]()

[Verificare se una stringa data è un palindromo. Attenzione alla Case Sensitivity. (Senior)]()

[Qual è la differenza tra uno Shim e un Polyfill? (Senior)]()

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

[Descrivi il concetto di Closure in JavaScript come meglio riesci. (Senior)]()

[Scrivi una funzione ricorsiva che restituisce la stringa binaria di un dato numero decimale. (Senior)]()

[Cos'è una Closure in JavaScript? Fornisci un esempio. (Expert)]()

[Spiegazione del concetto di Hoisting in Javascript. (Expert)]()

[Dato un intero, determinare se è una potenza di 2. In tal caso, restituire il suddetto numero, altrimenti -1. (Expert)]()

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

JavaScript mette a disposizione l'operatore `typeOf`, il quale esamina il valore dato e restituisce il tipo di dato.
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



[[↑] Back to top](#JavaScript)
### Spiegazione dei tipi di dato in JavaScript. (Mid)

JavaScript ha la tipizzazione dei dati ma non delle variabili. I seguenti tipi primitivi sono dipsponibili:
* `string`
* `number`
* `boolean`
* `null` e `undefined`
* `object`
* `symbol` (introdotto in ES6)



[[↑] Back to top](#JavaScript)
### Posto di avere un array non ordinato contenente (n - 1) di n numeri consecutivi (avendo definito i limiti) trovare il numero mancante mantenendo un tempo di esecuzione di O(n). (Mid)

```js
// L'output della funzione dovrebbe essere 8
var arrayOfIntegers = [2, 5, 1, 4, 9, 6, 3, 7];
var upperBound = 9;
var lowerBound = 1;

findMissingNumber(arrayOfIntegers, upperBound, lowerBound);     // 8

function findMissingNumber(arrayOfIntegers, upperBound, lowerBound) {
    // Iterarazione dell'array per calcolare la somma dei numeri
    var sumOfIntegers = 0;
    for (var i = 0; i < arrayOfIntegers.lenght; i++) {
        sumOfIntegers =+ arrayOfIntegers[i];
    }

    // Trovare la somma dei numeri consecutivi usando una variazione della somma di Gauss
    // Formula: [(N * (N + 1)) / 2] - [(M * (M - 1)) / 2];
    // N è il limite superiore ed M il limete inferiore

    upperLimitSum = (upperBound * (upperBound + 1)) / 2;
    lowerLimitSum = (lowerBound * (lowerBound - 1)) / 2;

    theoreticalSum = upperLimitSum - lowerLimitSum;

    return theoreticalSum - sumOfIntegers;
}
```

###### Source

* https://github.com/kennymkchan/interview-questions-in-javascript



[[↑] Back to top](#JavaScript)
### Rimuovere gli elementi duplicati da un array e restituire un nuovo array con gli elementi restanti. (Mid)

```js
// ES6
var array = [1, 2, 3, 5, 1, 5, 9, 1, 2, 8];

Array.from(new Set(array));     // [1, 2, 3, 5, 9, 8]

// ES5
var array = [1, 2, 3, 5, 1, 5, 9, 1, 2, 8];

uniqueArray(array);     // [1, 2, 3, 5, 9, 8]

function uniqueArray(array) {
  var hashmap = {};
  var unique = [];

  for(var i = 0; i < array.length; i++) {
    // Se la chiave è undefined (univocità) sarà false
    if(!hashmap.hasOwnProperty(array[i])) {
      hashmap[array[i]] = 1;
      unique.push(array[i]);
    }
  }

  return unique;
}
```

###### Source

* https://github.com/kennymkchan/interview-questions-in-javascript



[[↑] Back to top](#JavaScript)
### Data una stringa, invertire il verso di ogni parola. (Mid)

```js
var string = "Welcome to this Javascript Guide!";

// L'output sarà "!ediuG tpircsavaJ siht ot emocleW"
var reverseEntireSentence = reverseBySeparator(string, "");

// L'output sarà "emocleW ot siht tpircsavaJ !ediuG"
var reverseEachWord = reverseBySeparator(reverseEntireSentence, " ");

function reverseBySeparator(string, separator) {
  return string.split(separator).reverse().join(separator);
}
```

###### Source

* https://github.com/kennymkchan/interview-questions-in-javascript



[[↑] Back to top](#JavaScript)
### Scrivere una funzione che ti permetta di fare questo. (Mid)

Si può scrivere una *closure* per mantenere il valore passato alla funzione `createBase` anche dopo che la funzione interna verrà restituita. La funzione interna che viene restituita viene creata all'interno della funzione esterna, rendendola una *closure* e permettendole quindi l'accesso alle variabili all'interno della funzione esterna, in questo caso la variabile `baseNumber`.
```js
function createBase(baseNumber) {
    return function(N) {
        // Stiamo facendo riferimento alla variabile baseNumber anche se è dichiarata
        // all'esterno della funzione. Le Closure in JavaScript ti permettono di farlo
        return baseNumber + 1
    }
}

var addSix = createBase(6);
addSix(10);
addSix(21);
```

###### Source

* https://coderbyte.com/algorithm/3-common-javascript-closure-questions



[[↑] Back to top](#JavaScript)
### Implementare l'accodamento(enqueue) e l'estrazione(dequeue) di un elemento usando solamente due stack. (Mid)

*Accodare* significa aggiungere un elemento, *Estrarre* significa rimuoverlo.
```js
var inputStack = []     // Prima stack
var outputStack = [];   // Seconda stack

// Per l'accodamento ci basta aggiungere l'elemento nella prima stack
function enqueue(stackInput, item) {
  return stackInput.push(item);
}

function dequeue(stackInput, stackOutput) {
  // Invertiamo ora la stack facendo si che il primo elemento diventi l'ultimo
  // e viceversa
  // A questo punto rimuoviamo l'ultimo elemento dalla stack per restituire il primo
  // elemento inserito all'interno della stessa.
  if (stackOutput.length <= 0) {
    while(stackInput.length > 0) {
      var elementToOutput = stackInput.pop();
      stackOutput.push(elementToOutput);
    }
  }

  return stackOutput.pop();
}
```

###### Source

* https://github.com/kennymkchan/interview-questions-in-javascript



[[↑] Back to top](#JavaScript)
### Come usare una closure per creare un contatore di tipo private. (Mid)

Si può scrivere una funzione all'interno di un'altra funzione (*closure*) che permetta di aggiornare una variabile privata, senza però renderla accessibile all'esterno senza l'utilizzo di una funzione che venga in aiuto.
```js
function counter() {
    var _counter = 0;
    // Restituisco un oggetto con funzioni che permettono di modificare lo stato
    // della variabile _counter
    return {
        add: function(increment) { _counter += increment },
        retrieve: function() { return "Il contatore attualmente è a: " + _counter; }
    }
}

// Sarà dato errore nel caso in cui si provi ad accedere alla variabile _counter

// Utilizzo della funzione counter
var c = counter();
c.add(5);
c.add(9);

// Ora possiamo accedere alla variabile _counter nel seguente modo
c.retrieve();       // Il contatore attualmente è a: 14 
```

###### Source

* https://coderbyte.com/algorithm/3-common-javascript-closure-questions



[[↑] Back to top](#JavaScript)
### Spiegazione di Null e Undefined in JavaScript. (Senior)

JavaScript (e per estensione TypeScript) hanno due tipi di dato primitivi: `null` e `undefined`.
Questi, come vediamo, rappresentano due concetti differenti:
* Qualcosa non è stato inizializzato : `undefined`.
* Qualcosa non è attualmente disponibile : `null`.



[[↑] Back to top](#JavaScript)
### Spiegazione dell'Event Bubbling e del metodo per impedirlo. (Mid)

L'**Event Bubbling** è un concetto per il quale se un evento viene scatenato in un elemento annidato ad un altro elemento cosiddetto padre, anche l'evento dell'elemento padre sarà scatenato, proseguendo così per altri eventuali annidamenti.

Un metodo per prevenire l'*event bubbling* è tramite l'utilizzo di `event.stopPropagation()`  oppure `event.cancelBubble` in IE < 9.

###### Source

* https://github.com/kennymkchan/interview-questions-in-javascript



[[↑] Back to top](#JavaScript)
### Come verificare che un oggetto sia un array? (Mid)

Il metodo migliore per scoprire se un oggetto è un'istanza di una particolare classe o meno è tramite l'utilizzo del metodo `toString` della proprietà `Object.prototype`.
```js
var arrayList = [1, 2, 3];
```

Uno dei migliori casi d'uso per il controllo dei tipi di un oggetto è quando eseguiamo l'overloading dei metodi in JavaScript. Per capire al meglio questo concetto poniamo di avere un metodo chiamato `greet` che prende una singola stringa e una lista di stringhe.

Per permettere al nostro metodo `greet` di funzionare in entrambe le situazioni abbiamo bisogno di sapere la tipologia del parametro passato, se una singola stringa o una lista di stringhe.
```js
function greet(param) {
    if() {
        // Abbiamo bisogno di verificare se il parametro è un array o meno
    } else {

    }
}
```

Tuttavia, nell'implementazione sopra riportata potrebbe non essere necessario controllare se il parametro è un array, possiamo verificare per un singolo valore (in questo caso la stringa) e quindi implementare la logica per la gestione dell'array nel blocco *else*. Vediamo come fare di seguito.
```js
function greet(param) {
    if(typeof param === "string") {
        // TO DO
    } else {
        // Se il parametro è di tipo array allora questo blocco di codice sarà eseguito
    }
}
```

Ad ora potremmo rimanere tranqilli con le due implementazioni appena riportate, ma qualora il tipo di parametro, oltre a stringa e lista di stringhe, potesse essere un `object` ci troveremmo in difficoltà.

Per ovviare a questo problema, come abbiamo menzionato sopra, potremmo utilizzare `Object.prototype.toString`.
```js
if(Object.prototype.toString.call(arrayList) === "[object Array]") {
    console.log("Array!");
}
```

Se si sta utilizzando `jQuery` si può utilizzare il metodo proprietario `isArray`:
```js
if($.isArray(arrayList)) {
    console.log("Array!");
} else {
    console.log("Not array!");
}
```

FYI jQuery utilizza `Object.prototype.toString.call` internamente.

Nei browser più moderni (Chrome 5, Firefox 4.0, IE 9, Opera 10.5 e Safari 5) si può anche utilizzare:
```js
Array.isArray(arrayList);
```

###### Source

* https://github.com/ganqqwerty/123-Essential-JavaScript-Interview-Question/blob/master/README.md



[[↑] Back to top](#JavaScript)
### Scrivere una "mul" function (Funzione per moltiplicare). (Mid)
```js
function mul(x) {
    return function (y) {   // Funzione anonima
        return function (z) {   //Funzione anonima
            return x * y * z;
        };
    };
}
```
