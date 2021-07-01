# OPERADOR UNARIO

São operadores que trabalham com apenas um operando.

Operadores:

* `+`
  * 'mais'
    * Converte o operando em um número
* `-`
  * Converte o operando em um número negativo

* Ao converter uma string que não pode ser convertida em um número o js retorna um NaN. 

O incremento e o decremento é equivalente a uma operação de atribuição com a propria variável e uma unidade de valor

```js

let a = 10;
a = a + 1 // 11 
// mesma coisa que ++a
```

```js
let a = 10;
a = +a; // 10
a = -a; // -10
```

```js
// Convertendo String em número
// Mesma funcionalidade do Number();
let a = "30";
a = +a; //10
```

```js
// Convertendo Boleano em número
let falso = false;
let verdadeiro = true;
falso = +falso; // 0
verdadeiro = +verdadeiro; // 1
```

```js
let salario = 500;
let dia seguinte = -salario; // -500
```

*  `++`
   *  Incremento
      *  Acrescenta uma unidade de valor ao operando.
      * Existe dois tipos, prefixo e posfixo
        * prefixo: ++a
          * Antes de qualquer operação o acrescimo é realizado.
*  `--`
   *  Decremento
      * Diminui uma unidade de valor do operando.
      * Existe dois tipos, prefixo e posfixo
        * prefixo: --a
          * Antes de qualquer operação o acrescimo é realizado.
        * posfixo: a++
          * Apos todas a operações e execuções da linha o acrescimo e executado. 
        * posfixo: a++
          * Apos todas a operações e execuções da linha o acrescimo e executado. 

```js
// incremento prefixo
let i = 10;
++i; // 11;
```

```js
// incremento posfixo
let i = 10;
let j = 5;
let soma = i++ + j; // 15;
// i = 11; o acrescimo acontece após a soma.
 ```

```js
// decremento prefixo
let i = 10;
--i; // 9;
```

```js
// decremento posfixo
let i = 10;
let j = 5;
let soma = i-- + j; // 15;
// i = 9; o acrescimo acontece após a soma.
 ```