# JAVA SCRIPT

## JQUERY
` jQuery offers a simple way to achieve a variety of common JavaScript tasks quickly and consistently`
* SELECT ELEMENTS
* PERFORM TASKS
* HANDLE EVENTS
![JQUERY](https://e7.pngegg.com/pngimages/639/1023/png-clipart-logo-jquery-in-easy-steps-create-dynamic-web-pages-brand-ajax-jquery-logo-blue-text.png)

### WHY USE JQUERY
* SIMPLE SELECTORS
  *  Are much faster at selecting elements
  * Can be a lot more accurate about which elements to select
  * Often require a lot less code than older DOM
methods
  * Are already used by most front-end developers

* COMMON TASKS IN LESS CODE
  * loop through elements
  *  Add I remove elements from the DOM tree
  * Handle events
  * Fade elements into I out of view
  * Handle Ajax requests
  ![selector](https://i1.wp.com/www.admecindia.co.in/wp-content/uploads/2020/01/jquery-selectors.png?resize=318%2C196&ssl=1)

### LOOPING
* when a selector
returns multiple elements, you
can update all of them using the
one method
![loop](https://i.ytimg.com/vi/J9YSCqg5MI4/hqdefault.jpg)

### CHAINING
* The process of placing several
methods in the same selector is
referred to as chaining. As you
can see, it results in code that is
far more compact.</br>
`<script>`
`    $(document).ready(function () {`
`        $('input').change(function () {`
`            alert(this.value);`
`        });`
`    });`
`</script>`

### updating element
* `.html()`
  
  * This method gives every element in the matched set the same new content. The new content may include HTML

* `.text()`

  * This method gives every element in the matched set the same new text content. Any markup would be shown as text.

* `.replaceWith()`

  * This method replaces every element in a matched set with new content. It also returns the replaced elements.

* `.remove()`

  * This method removes all of the elements in the matched set.

  ### INSERTING ELEMENTS
* `.before()`

  * This method inserts content before the selected element 

* `.after()`

  * This method inserts content after the selected element 

* `.prepend()`

  * This method inserts content inside the selected element after the opening tag.

* `.append()`

  * This method inserts content inside the selected element, before the closing tag.

## LOADING JQUERY FROM A CDN
![CDN](https://www.yogihosting.com/wp-content/uploads/2017/12/jquery-cdn.jpg)

`<script src=" //ajax .googl eapi s . com/ ajax/l i bs/ jquery / 1.10 . 2/ jquery .min. js "> </ script>`
</br>
`<script>` 
`window .jQuery 11 document. write (' <script src=" j s/j query- 1.10. 2 . j s 11><\jscri pt> ' )`
`</script>`
