[BACK](https://abdullahmou.github.io/reading-notes/)
# CSS

## flexbox

* Properties for the Parent
  * display
  
    * `.container {  display: flex; /* }`
  
  * flex-direction
    
    * `.container {flex-direction: row | row-reverse | column | column-reverse;}`
  
  * flex-wrap
    * `.container { flex-wrap: nowrap | wrap | wrap-reverse;}`

  * flex-flow
    * `.container { flex-flow: column wrap;}`

  * justify-content
    * `.container {`
      `justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;`
      `}`

  * align-items
    * `.container {`
   `align-items: stretch | flex-start | flex-end | center | baseline | first baseline | last baseline | start | end | self-start | self-end + ... safe | unsafe;`
    `}`

  * align-content
    * `.container {`
   `align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch | start | end | baseline | first baseline | last baseline + ... safe | unsafe;`
   `}`
</br> </br>

* Properties for the Children

  * order
    * `.item {  order: 5; /* default is 0 */}`

  * flex-grow
    * `.item {  flex-grow: 4; /* default 0 */}`

  * flex-shrink
    * `item {  flex-shrink: 3; /* default 1 */}`
  
  * flex-basis
    * `.item {  flex-basis:  | auto; /* default auto */}`

  * flex
    * `.item {  flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ]}`

  * align-self
    * `.item {  align-self: auto | flex-start | flex-end | center | baseline | stretch;}`

</br> </br>

# JavaScript

## Templating

* Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
![Templating](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQrhrkvjhqhCXmieLqeCI46bIfANw9_GbMmkA&usqp=CAU)

* Mustache-Express
  * If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily.
  ![express](https://miro.medium.com/max/875/1*LbqYj87xlazySm6wE0Q2lA.png)

  ![mustache](https://miro.medium.com/max/875/1*P9q0tkeaRY2l1JOXaVKAig.png)
  
