<h1>Server for autotesting api</h1>
You can query, add, delete and modify the list of books

<h2>How to start</h2>

1. npm install
2. npm install -g nodemon
3. nodemon app.js

<h2>Requests</h2>

<hX>Base Url</hX>
<ul><li><b>http://localhost:3000</b></li></ul>

<hX>Endpoints</hX>
<ul>
  <li>GET: get books: <b>&ensp;/books/</b></li>
  <li>GET: get book by id: <b>&ensp;/books/:id</b></li>
  <li>POST: add book: <b>&ensp;/books/</b></li>
  Body: 
  <p><code>{
    "author":"Douglas Adams",
    "id":"1",
    "title":"The Hitchhiker's Guide to the Galaxy"
}</code></p>
  <p>or</p>
  <p><code>{
    "author":"Douglas Adams",
    "title":"The Hitchhiker's Guide to the Galaxy"
    }</code></p>
  <p>id can be omitted, it will be generated automatically(as an example: "543c3fe5-387d-45b3-b36d-99525eab3ae2")</p>
  <li>PUT: update book by id: <b>&ensp;/books/:id</b></li>
  Body: <p><code>{
    "title": "title",
    "author": "author"
  }</code></p>
  <li>DELETE: delete book by id: <b>&ensp;/books/:id</b></li>
</ul>
