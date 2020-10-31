[BACK](https://abdullahmou.github.io/reading-notes/)

# EJS

## Where is EJS used

* EJS is used in node.js when working with the Express framework as a templating engine to help render JavaScript code on the client-side.
![](https://miro.medium.com/max/720/1*DG4VA127mu4Fx2TrRIzskw.jpeg)


## what is EJS

* a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

* stands for embedded JavaScript. It lets us embed JavaScript code (variables, if statement, loops) inside of our HTML

![ejs](https://miro.medium.com/max/850/1*usicWavHRKy4Sjm2XTCBMA.jpeg)

## how dose it work

* install package
  * `npm install ejs --save express`

* Set EJS as templating engine
  * ` var express = require('express'); `</br>
      `var app = express(); `</br>
     `app.set('view engine', 'ejs'); `

* make a file named “home.ejs”
  * `<!DOCTYPE html>` </br>
`<html> `</br>
  `<head>     <title>Home Page</title> </head> `</br>
  `<body>   <center>This is our home page.</center> </body> `</br>
`</html> `

* render this page 
  * `app.get('/', (req, res)=>{ `</br>
    ` res.render('home'); `</br>
      `}); `

* add dynamic content render method
  * `app.get('/', (req, res)=>{ `</br>
  `res.render('home', {name:'Akashdeep'}); `</br>
`});`   </br>
`var server = app.listen(4000, function(){ `</br>
 `   console.log('listining to port 4000') `</br>
`});` 

* embed name to HTML page 
  * `<!DOCTYPE html>` </br>
`<html> `</br>
  `<head>     <title>Home Page</title> </head> `</br>
  `<body>  `</br>
    ` <center>`</br>
     `This is our home page.<br>`</br>
     ` Welcome <%=name%>, to our home page.`</br>
    `</center>`</br>
  ` </body> `</br>
`</html> `

* embedding loop for (li)
  * in server.js
    * `app.get('/', (req, res)=>{ `</br>
`var data = {name:'Akashdeep', `</br>
`    hobbies:['playing football', 'playing chess', 'cycling']} `</br>
`res.render('home', {data:data}); `</br>
`}); `</br>
`var server = app.listen(4000, function() { `</br>
`    console.log('listining to port 4000') `</br>
`});` 
  * in HTML.ejs
    * `<body> `</br>
`    Hobbies of <%=data.name%> are:<br/> `</br>
`    <ul> `</br>
`        <% data.hobbies.forEach((item)=>{%> `</br>
`        <li><%=item%></li>  `</br>
`        <%});%> `</br>
`    </ul> `</br>
`</body>`

  * result:</br>
    * ![](https://media.geeksforgeeks.org/wp-content/uploads/20190625162033/ejs.png)
