[BACK](https://abdullahmou.github.io/reading-notes/)

# Call stack

* A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function

![](https://image.slidesharecdn.com/sonlejs-event-loop-160805060652/95/javascript-event-loop-13-638.jpg?cb=1470377352)</br>
  * When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
  * Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
  * When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
  * If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error

# error messages
![](https://i.stack.imgur.com/i3Im2.png)</br>

## Types of error messages

![](https://cdn2.hexlet.io/derivations/image/original/eyJpZCI6Ijg4NDgzMDE5ZjVlNGJkZTZhOGE3YTcxM2Q2MGRiZTk5LnBuZyIsInN0b3JhZ2UiOiJjYWNoZSJ9?signature=8041732636e435d842d9e2369e8c9704014c499882461b192fab65421e35d36f)</br>

* Reference errors
  * errors :</br>
  ` console.log(foo) // Uncaught ReferenceError: foo is not defined `</br></br>
   `foo = 'Hello' // Uncaught ReferenceError: foo is not defined let foo`

* Syntax errors
  * errors :</br>
   `JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1`</br></br>
   `JSON.parse('{"foo":"bar"}')`</br>

* Range errors
  * errors :</br>
  `var foo= []`</br>
`foo.length = foo.length -1 // Uncaught RangeError: Invalid array length ` </br></br>
`var foo = [0, 0]`</br>
`foo.length = foo.length - 2 // (or foo.length - foo.length)`</br>
`foo // would log [] instead of [0, 0]`</br>

* Type errors
  * errors :</br>
  `var foo = {}`</br>
`foo.bar // undefined`</br>
`foo.bar.baz // Uncaught TypeError: Cannot read property 'baz' of undefined`</br></br>
`var foo = { bar: {} }`</br>
`foo.bar.baz // undefined but you avoid the error`</br>

# Debugging

![](https://image.slidesharecdn.com/debugging-javascript-web-141030080414-conversion-gate02/95/debugging-javascript-1-638.jpg?cb=1415345877)
