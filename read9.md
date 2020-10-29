[BACK](https://abdullahmou.github.io/reading-notes/)

# Concepts of Functional Programming

## What is functional programming

* Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data
![](https://www.leadingagile.com/wp-content/uploads/2018/02/When-functional-programming-isnt.jpg)

## Pure functions

![](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSyOX6Lp_V_4Itx6WtKNDdIYmiHaKhbPrXz_A&usqp=CAU)
* It returns the same result if given the same arguments
  * ` let PI = 3.14; `
    ` const calculateArea = (radius) => radius * radius * PI; `
    ` calculateArea(10); // returns 314.0 `
* It does not cause any observable side effects
  * `let counter = 1;`
    `function increaseCounter(value) {`
    `counter = value + 1;}`
    `increaseCounter(counter);`
    `console.log(counter); // 2`

## Immutability

![](https://miro.medium.com/max/1200/1*mA2NV6aiBt4iVKFGqFmy5g.jpeg)
* When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

## Referential transparency

![](https://edward-huang.com/images/pure-function-vs-referential-transparency/Pure%20vs%20Referential%20Transparent.png)
* Basically, if a function consistently yields the same result for the same input, it is referentially transparent.
  * ` pure functions + immutable data = referential transparency `

# Refactoring

![](https://miro.medium.com/max/1116/1*1fGgnh-krPxk4o5343J5Vg.png)

## Standards

* There is no doubt that standards help to improve the quality of code. It’s important to check for those standards while refactoring your code

* Introduce Parameter

  * before :</br>
  ` function calculate_sum(i) {`</br>
 `   alert('Adding ' + 1 + ' to ' + i);`</br>
`    return 1 + i;}`</br>
`function show_sum() {`</br>
 `   alert('Result: ' + calculate_sum(5));}`


  * after :</br>
  ` function calculate_sum(i, i2) {`</br>
`    alert('Adding ' + i2 + ' to ' + i);`</br>
`    return i2 + i;}`</br>
`function show_sum() {`</br>
`    alert('Result: ' + calculate_sum(5, 1));} `</br>


* Introduce a parameter

  * ![](https://resources.jetbrains.com/help/img/idea/2020.2/ws_js_extract_parameter_result.png)


* Introduce Variable
  * before :</br>
  ` Parenizor.method('toString', function ()){`</br>
  `  return '(' + this.getValue() + ')';}`

  * after :</br>
  ` Parenizor.method('toString', function ()){`</br>
    `let string = '(' + this.getValue() + ')';`</br>
   ` return string;}`

![](https://img1.pnghut.com/19/11/2/sMbuYaCsJq/computer-programming-javascript-code-refactoring-logo-communication.jpg)
