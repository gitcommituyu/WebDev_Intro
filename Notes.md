# Un vistazo al desarrollo web

## Introducción
* En esta parte realizaremos un repaso a los conceptos clave del desarrollo web; este taller está pensando de tal manera que, sin importar el nivel de conocimientos que posean, podamos refrescar la memoria, o aprender un nuevo concepto o herramienta para aplicar en nuestro próximo proyecto.

## HTML
* Empezaremos con Hypertext Markup Language o más bien conocido como **HTML** por sus siglas.
* HTML es nuestro esqueleto para la creación de páginas web, las cuales Safari, Google Chrome o Firefox interpretan en nuestras pantallas.
* Para poder crear una página web básica:
  ```html
  <!DOCTYPE html>
  <html>
     <head>
         <title>Hola</title>
     </head>
     <body>
         Hola Mundo!
     </body>
  <html>
  ```
* Si así lo preferimos, podemos visualizar nuestra página creada con un Document Object Model o DOM por sus siglas en inglés. Acá podemos ver nuestro DOM de la página creada anteriormente.
![image](https://github.com/gitcommituyu/WebDev_Intro/assets/81819758/52019190-e6df-43d0-bdce-27fe58d72bd9)
* Pero nuestra página se ve bastante simple. Podemos agregar más complejidad a nuestras páginas utilizando elementos en HTML.

  ```html
  <!DOCTYPE html>
  <html lang="en">
     <head>
         <title>HTML Elements</title>
     </head>
     <body>
         <!-- We can create headings using h1 through h6 as tags. -->
         <h1>A Large Heading</h1>
         <h2>A Smaller Heading</h2>
         <h6>The Smallest Heading</h6>
  
  
         <!-- The strong and i tags give us bold and italics respectively. -->
         A <strong>bold</strong> word and an <i>italicized</i> word!
  
  
         <!-- We can link to another page (such as cs50's page) using a. -->
         View the <a href="https://cs50.harvard.edu/">CS50 Website</a>!
  
  
         <!-- We used ul for an unordered list and ol for an ordered one. both ordered and unordered lists contain li, or list items. -->
         An unordered list:
         <ul>
             <li>foo</li>
             <li>bar</li>
             <li>baz</li>
         </ul>
         An ordered list:
         <ol>
             <li>foo</li>
             <li>bar</li>
             <li>baz</li>
         </ol>
     </body>
  <html>
  ```

## CSS
* Cascading style sheets o **CSS** por sus siglas en inglés es nuestro lenguaje para poder hacer que nuestras páginas se vean bien bonitas.
* Hay múltiples maneras de hacer que una página se vea bonita y podemos entrar en múltiples niveles de profunidad, pero con lo básico podemos agregar estilo:
  ```html
  <h1 style="color: blue; text-align: center;">A Colorful Heading!</h1>
  ```
* Pero podemos hacerlo mejor, para que sea más limpio, podemos agregar un tag de `style` en nuestro `head`_
  ```html
  <style>
   h1 {
       color: blue;
       text-align: center;
   }
  </style>
  ``
* Incluso utilizando selectores y clases, como en este caso la clase .boton-rojo
```html
<style>
.boton-rojo {
   background-color: red;
   color: white;
   padding: 10px 20px;
   border: none;
}
</style>

<!-- HTML -->
<button class="boton-rojo">Click Me</button>
```

## JavaScript
* Pero por muy bonita que sea nuestra página, quizás nosotres queremos que también responda al usuario.
* Mientras que antes el usuario estaba realizando consultas al servidor, con Javascript podremos generar funcionalidades desde el dispositivo del usuario.
* Para crear nuestro script básico con JavaScript podemos:
  ```html
  <script>
     alert('Hello, world!');
  </script>
  ```
* Pero podemos hacer mejor que esto utilizando funciones:
  ```html
  <script>
     function hello() {
         alert('Hello, world!')
     }
  </script>
   <!-- HTML -->
  <button onclick="hello()">Click Here</button>
  ```
* O incluso mejor si utilizamos variables
  ```html
   <script>
       let counter = 0;
       function count() {
           counter++;
           alert(counter);
       }
   </script>
    <!-- HTML -->
   <button onclick="count()">Count</button>
  ``

* Incluso podemos utilizar esto para cambiar nuestro DOM
  ```html
  <script>
     let counter = 0;
     function count() {
         counter++;
         document.querySelector('h1').innerHTML = counter;
     }
   </script>
  ```
## ¡Ahora les toca a vosotros!
Es vuestro turno de realizar una página web.




