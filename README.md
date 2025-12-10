# LM-PRUEBA-R2-RLM-1-DAM

## Informe de Evidencias

## Ejercicio 1


### 1A. Pregunta
### ¿Por qué NO se centra el texto del 'h1' en este caso? Explícalo con tus palabras. (por qué visual y estructuralmente no aparece centrado entre el borde izquierdo y el menú)

Ya que estás colocando el h1 aparte del .site-header y este h1 debería estar enlazado de alguna manera con el .site-header para que gracias al flex pueda centrarse el texto. Entonces, con el text-align no es suficiente para centrarlo

Debería colocarse de la siguiente manera para que el flex haga efecto sobre él:

".site-header h1 {

  text-align: center;
  
}"


### 1B. Ejercicio: Soluciona de dos formas diferentes

Primero veremos como podemos arreglar esto con flex:

<img width="360" height="332" alt="image" src="https://github.com/user-attachments/assets/aaec5d27-d971-44a2-b0eb-52cad260267e" />

Como podemos observar, el h1 está unido al .site-header y como en él están los ajustes del flex, el h1 se encuentra centrado en el texto.

Ahora veremos el caso con grid:

<img width="292" height="290" alt="image" src="https://github.com/user-attachments/assets/9eb1c6e0-c2c7-4a40-be75-4075627f14b0" />

Aquí podemos observar que el grid se encarga de centrar el h1 y las opciones quedan por debajo del h1 como la siguiente imagen:

<img width="937" height="323" alt="image" src="https://github.com/user-attachments/assets/1e1867d2-2b28-4951-87b4-633dcae5eba2" />


### 1C. Ejercicio: Convertir la cabecera en dos filas

<img width="395" height="469" alt="image" src="https://github.com/user-attachments/assets/c6834f32-d105-4843-ac42-59d01045d846" />


### 1D. Ejercicio: Dar relieve y separación visual al header

<img width="386" height="349" alt="image" src="https://github.com/user-attachments/assets/6ac117d9-4d11-41a3-a7d0-6c6ab960e681" />

<hr>

## Ejercicio 2: Reorganización del header con tres elementos


### 2A. Ejercicio

<img width="617" height="586" alt="image" src="https://github.com/user-attachments/assets/8e7b932f-ff5f-406d-b4ac-35ba149fe779" />

### 2B. Ejercicio 

Como se ve ahora la página: 
<img width="1920" height="305" alt="image" src="https://github.com/user-attachments/assets/b69e0a48-d387-4862-94ad-460ee5a1cf89" />

CSS:

<img width="328" height="645" alt="image" src="https://github.com/user-attachments/assets/4bcd93c9-a8cc-4dfd-934b-7375bda1bf71" />

<img width="402" height="298" alt="image" src="https://github.com/user-attachments/assets/3d4a76bf-14ab-4aea-bfb1-29676533995d" />

<hr>

## Ejercicio 3
### 3A. Crear miniaturas

<img width="552" height="348" alt="image" src="https://github.com/user-attachments/assets/b9d67406-cf95-477b-80ee-4714caed5f4c" />

<img width="531" height="167" alt="image" src="https://github.com/user-attachments/assets/05cf0933-d057-46e5-968b-98c80afdb662" />


### 3B. Efecto hover

<img width="294" height="272" alt="image" src="https://github.com/user-attachments/assets/a4dcd6ac-c454-4b05-9e88-33bb2b3a20d5" />


### 3C. Enlace a la imagen original 

<img width="920" height="674" alt="Captura de pantalla 2025-12-09 135206" src="https://github.com/user-attachments/assets/4d93e296-0a00-4f3f-92ba-9fbcdfc948eb" />


<img width="952" height="919" alt="image" src="https://github.com/user-attachments/assets/8d5461c8-610f-4be1-9478-42718b3a18d3" />

<hr>

## Ejercicio 4: Informe de evidencias del proyecto (defensa técnica simple)

### 4.1. Introducción

Para esta prueba, decide crear una página web centrada en uno de mis videojuegos favoritos: Time Traveler. Para la página decide incluir una pequeña sipnosis sobre la narrativa del juego, una galería de imágenes que contiene algunas imágenes del juego, una tabla con las especificaciones del juego, como lo serían el nombre de la creadora, el año de publicación...
Luego podemos encontrar un formulario para contactarse con la desarrolladora de la página para saber más del juego y por último encontramos diversos links sobre las redes sociales y la página donde se descargan los de la creadora. 

Para el diseño de la página he tomado la paleta de colores del juego, en el que se destaca mucho tonos de color azul. En el header decidí colocar algunos sprites del juego para representar a los personajes más importantes en su narrativa. Se buscaba respetar mucho los espacios para que se aprecie más lo visual de la página. Para el botón de la parte superior izquierda decidí utilizar unos assets del juego de la protagonista con el ojo abierto y cerrado si se abre. 

### 4.2. Evidencias de HTML5

1. Header
   
En el header, con una class "site-header", podemos encontrar el título de la página dentro de un h1, luego los sprites de los personajes más importantes del juego que se encuentran dentro de un figure. Después encontramos un nav con class "main-nav" que hace referencia a las diferentes secciones de la página para poder acceder a ellas mediante enlaces. A continuación tenemos un botón que sirve para el menú lateral, que funciona con JavaScript y por último encontramos otro nav con id "sideMenu" y un class "side-menu". En este otro nav se utiliza para el menú lateral el cual tiene unos enlaces que nos llevan a cada sección de la página, al igual que el primer nav.

```html
<header class="site-header">
    <h1>Time Traveler</h1> 
    <figure>
      <img src="img/mai1.png" alt="1" class="chibi">
      <img src="img/kyo1.png" alt="2" class="chibi">
      <img src="img/kazu.png" alt="3" class="chibi">
      <img src="img/sakura.png" alt="4" class="chibi">
      <img src="img/chrono.png" alt="5" class="chibi">
      <img src="img/pietro.png" alt="6" class="chibi">
    </figure>
    
    <nav class="main-nav">
        <a href="#hero">Inicio</a>
        <a href="#galeria">Galería</a>
        <a href="#tab">Tabla</a>
        <a href="#for">Formulario</a>
        <a href="#con">Contacto</a>
    </nav>

    <button class="open-menu" aria-label="Abrir menú lateral"><img id="toggleIcon" src="img/boton.png"></button>

    <nav id="sideMenu" class="side-menu">
        <a href="#hero">Inicio</a>
        <a href="#galeria">Galería</a>
        <a href="#tab">Tabla</a>
        <a href="#for">Formulario</a>
        <a href="#con">Contacto</a>
    </nav>
  </header>
```

Así es como se vería en la página: 
![Header](img/header.png)
![MenuLateral](img/menuLateral.png)

En el header podemos encontrar los siguientes enlaces internos:
![EnlaceHeader](img/enlaces1.png)
![EnlaceMenuLateral](img/enlaces2.png)

2. Main


El main, que es donde se recoge todo el contenido de la página web, se encuentra compuesto por todas las secciones que podemos encontrar en la página web, por lo tanto, iremos sección por sección viendo cada una de ellas:

2.1. Section Hero

  
Este primer section, con id "hero", encontramos otro header el cual sirve para el título de la sección.         Luego, encontramos un article el cual abarca todo el texto y la imagen que se encuentran ahí. Hay un h3 para    el subtítulo del texto que hay a continuación marcado por las etiquetas p. Por último encontramos un figure     que muestra la imagen de inicio del videojuego. 
  
```html
  <section id="hero">
      <header>
        <br>
        <h2>¡Bienvenido al mundo de Time Traveler!</h2>
        <br>
      </header>
      <article>
        <h3>Sinopsis</h3>
        <hr>
        <p>La joven <strong>Mizuno Mai</strong> es el resultado de la relación entre un espíritu y un ser humano. Ella se encuentra desde el principio de su vida atrapada en muchos misteriosos y curiosos mundos donde en cada uno hay seres, llamados <strong><em>Guardianes</em></strong>.</p>
        <p>Pero su nacimiento rompió las reglas de <strong>Dios</strong>. Y su abuelo está detrás de ella en orden de borrar su existencia y todo alrededor de ella.</p>
        <p>Debido a esto, con un poco de ayuda ella será capaz de viajar al <strong>pasado</strong>, <strong>presente</strong> y <strong>futuro</strong>, y necesitará crecer en muchas maneras para enfrentar sus miedos</p>
        <br>
        <figure>
              <img src="img/intro.png" alt="Intro de TT">
        </figure>
        <br>
      </article>
    </section>
```

  Así es como se vería en la página: 
  ![Hero](img/hero1.png)



    
  2.2. Section Galería de Imágenes

    
Para esta sección, encontramos la galería, el cúal consiste en un h2 como título de la sección y un figure      donde contiene todas las imágenes de la galería. A su vez, las imágenes tienen un enlace para que puedas        abrir la imagen original. 
  
```html
<section id="galeria">
      <br><br>
      <h2>Galería de imágenes</h2>
      <br><br>
      <figure>
        <a href="img/img4.png"><img src="img/img4.png" alt="1"></a>
        <a href="img/img5.png"><img src="img/img5.png" alt="2"></a>
        <a href="img/img6.png"><img src="img/img6.png" alt="3"></a>
        <a href="img/img7.png"><img src="img/img7.png" alt="4"></a>
        <a href="img/img8.png"><img src="img/img8.png" alt="5"></a>
        <a href="img/img1.png"><img src="img/img1.png" alt="6"></a>
        <a href="img/img2.png"><img src="img/img2.png" alt="7"></a>
        <a href="img/img3.png"><img src="img/img3.png" alt="8"></a>
        <a href="img/img9.png"><img src="img/img9.png" alt="9"></a>
      </figure>
      <br><br>
    </section>
```

Así es como se vería en la página: 
![Galeria](img/galeria.png)


En está sección, podemos encontrar los siguientes enlaces internos:
![EnlaceGalEj](img/enlacesEjGal.png)

  
2.3. Section Tabla/Especificaciones

En está sección, encontramos la tabla, la cúal tiene un h2 como título de la sección y a contnuación hacemos una tabla que se empieza con la etiqueta table y dentro de ella colocamos un tr por cada fila que hagamos. Dentro de cada tr, ponemos tantos th por cada columna que vayamos a colocar en la tabla. No podemos olvidarnos de que debemos espeficiar con colspan la cantidad de datos que vamos a colocar, en este caso siempre serán 2.

```html
<section id="tab">
      <br>
      <h2>Especificaciones</h2>
      <br><br>
        <table>
          <tr>
            <th colspan="2">Creadora</th>
            <th>Commodorette</th>
          </tr>
          <tr>
            <th colspan="2">Origen</th>
            <th>Argentina</th>
          </tr>
          <tr>
            <th colspan="2">Año de Publicación</th>
            <th>2015</th>
          </tr>
          <tr>
            <th colspan="2">Género</th>
            <th>Aventura Misterio</th>
          </tr>
          <tr>
            <th colspan="2">Creado con</th>
            <th>RPG Maker 2003</th>
          </tr>
          <tr>
            <th colspan="2">Duración</th>
            <th>8 horas</th>
          </tr>
          <tr>
            <th colspan="2">Última Actualización</th>
            <th>Febrero 2017</th>
          </tr>
          <tr>
            <th colspan="2">Sala Bonus</th>
            <th>Sí</th>
          </tr>
          <tr>
            <th colspan="2">Finales</th>
            <th>2 Finales (Bueno y Malo)</th>
          </tr>
          <tr>
            <th colspan="2">Traducción</th>
            <th>Español e Inglés</th>
          </tr>
        </table>
     <br>
    </section>
```


Así es como se vería en la página: 
![Tabla](img/tabla.png)


  
2.4. Section Formulario

En está sección, encontramos el formulario, el cúal tiene un h2 como título de la sección y debemos abrir dos etiquetas necesarias para que el formulario funciones: form y fieldset.

Dentro de fielset, colocamos la etiqueta legend, la cual es el título del formulario. Luego, para crear el campo que indicará el nombre de los datos necesario para el formulario es label y dentro de él, ponemos for, que funciona como un id. Después tenemos que indicar que se coloca en ese campo que lo hacemos con la etiqueta input. 

En input, debemos colocar id y name con el mismo nombre que el for y el type debe endicar que datos se esperar colocar ahí, por ejemplo, text para texto, email para correos y es necesario el @...

Por último, fuera de fieldset, ponemos los botones para poder enviar o borrar el formulario. Al igual que el anterior input, debemos poner el type, que en el caso de enviar, cuando se pulse el botón, recargará la página y el value es el texto que se verá en la página.

```html
<section id="for">
      <br>
      <h2>Formulario</h2>
        <h3>¿Quieres saber más sobre Time Traveler?</h3>
        <br>
        <form>
          <fieldset>
            <br>
            <legend>Datos</legend>
            <label for="nombre">Nombre</label>
            <input type="text" id="nombre" name="nombre" required>
             <label for="email">Email</label>
            <input type="email" id="email" name="email" placeholder="ejemplo@correo.com" required>
            <label for="telefono">Teléfono</label>
            <input type="tel" id="telefono" name="telefono" maxlength="15" placeholder="+34 11111111" required>
          </fieldset>
          <input type="submit" value="Envíar" class="boton">
          <input type="reset" value="Borrar" class="boton">
        </form>
    </section>
```

Así es como se vería en la página: 
![Formulario](img/form.png)


  
2.5. Section Contacto

En está última sección, encontramos el contacto, el cúal tiene un h2 como título de la sección y encontramos una lista desordenada que se abre con la etiqueta ul y li indica los componentes de esa lista. Aquí encontramos los enlaces a las redes sociales de la creadora del juego. Aquí es donde acaba el main.

```html
<section id="con">
      <br>
      <h2>Contacta a Commodorette</h2>
          <ul>
            <li><a href="https://x.com/Commodorette?s=20">Twitter/X</a></li>
            <li><a href="https://www.tumblr.com/rimururu">Tumblr</a></li>
            <li><a href="https://www.instagram.com/commodorette?igsh=bXY5ZTVtYXViZXB4">Instagram</a></li>
            <li><a href="https://commodogames.wordpress.com/">Página Oficial de Descarga de sus Juegos</a></li>
          </ul>
    </section>
```


Así es como se vería en la página: 
![Contacto](img/contc.png)

En esta sección podemos encontrar los siguientes enlaces externos:
![EnlaceContacto](img/enlaces3.png)

3. Footer

Aquí podemos encontrar el footer, el cúal presenta un class llamado "site-footer" y una línea el cual indica quien creo la página, de que curso es y el año de creación. En está línea podemos encontrar que funciona como enlace para que puedas volver arriba de la página. 

```html
<footer class="site-footer">
    <p><a href="#">&copy; 2025 — 1º DAM, Rocío Lobato Monferrer</a></p>
  </footer>
```


Así es como se vería en la página: 
![Footer](img/footer.png)

En el footer podemos encontrar el siguiente enlace interno:
![EnlaceFooter](img/enlaces4.png)


### 4.3. Evidencias de CSS

Este sería el CSS utilizado para esta práctica:

```css
/* ===== RESET CSS básico ===== */
*, *::before, *::after {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* ===== FONTS NECESARIOS ===== */

@font-face {
  font-family: "Título h1";
  src: url("fonts/Digital\ Change\ Demo.ttf") format('truetype');
} 

@font-face {
  font-family: "Opciones";
  src: url("fonts/Blackney-Bold.ttf") format('truetype');
}

@font-face {
  font-family: "text";
  src: url("fonts/Petrona-VariableFont_wght.ttf") format('truetype');
}

/* ===== ESTILOS BASE ===== */
body {
  font-family: system-ui, -apple-system, "Segoe UI", sans-serif;
  background-color: #31798c;
}

main {
    width: min(1100px, 90%);
    margin: 20px auto;
    background-color: #39aec6;
    box-shadow: 3px 14px 19px 22px #2e546e99;
}

p {
  font-family: "text";
  margin: 15px;
  font-size: 20px;
}

hr {
  width: 65%;
  margin: auto;
  border: #8cdbd6 solid 2px;
}

/* ===== CABECERA Y MENÚ SUPERIOR ===== */
.site-header { 
  position: sticky;
  top: 0;
  z-index: 10;
  background-color: #21556b;
  display: flex;
  align-items: center;
  color: #bde3de;
  padding: 20px;
}

.site-header h1 {
  font-family: "Título h1";
  margin: 30px auto;
  padding: 30px;
  text-align: center;
}

.main-nav ul {
  list-style: none;
  display: flex;
  gap: 10px;
}

.main-nav a {
  color: #bde3de;
  padding: 10px;
  font-family: "Opciones";
  text-decoration: none;
  display: flex;
  flex-direction: row;
  justify-content: right;
}

.main-nav a:hover {
  color: whitesmoke;
}

.site-header figure {
  margin: 10px;
}

.chibi:hover {
  transform: scale(1.03);
}

/* ===== BOTÓN HAMBURGUESA PARA GESTIONAR EL MENÚ LATERAL ===== */

.open-menu {
  position: fixed;
  top: 14px;
  left: 14px;
  z-index: 20;
  font-size: 26px;
  cursor: pointer;
  background: none;
  border: none;
  transition: transform 0.3s ease, background-color 0.3s ease;
}

/* ===== MENÚ LATERAL DESLIZANTE ===== */
.side-menu {
  position: fixed;
  top: 0;
  left: -230px;            
  width: 230px;
  height: 100%;
  background-color: #8cdbd6;
  padding-top: 60px;
  transition: left 0.3s ease;
  z-index: 15;
  font-family: "Opciones";
  display: flex;
  flex-direction: column;
}

.side-menu.active {
  left: 0;   
}

.side-menu ul {
  list-style: none;
  padding: 0;
}

.side-menu a {
  display: block;
  padding: 12px 20px;
  color: #31798c;
  text-decoration: none;
}

.side-menu a:hover {
  color: whitesmoke;
}

/* ===== HERO ===== */

#hero figure img {
    height: auto;
    margin: auto;
    display: block;
    width: 80%;
    object-fit: cover;
    border-radius: 10px;
}

/* ===== TITULOS ===== */

h2 {
  font-family: "Press Start 2P", system-ui;
  font-weight: 400;
  font-style: normal;
  width: 100%;
  margin: 20px;
}

h3 {
  margin: 15px;
  font-family: "Press Start 2P", system-ui;
  font-weight: 400;
  font-size: 20px;
  width: 100%;
  font-style: normal;
}

/* ===== GALERÍA ===== */

#galeria figure {
  display: grid;
  grid-template-rows: repeat(auto-fill, minmax(200px, autofr));
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 20px;
}

#galeria img {
    width: 80%;
    height: auto;
    object-fit: cover;
    border-radius: 10px;
    margin: auto;
    display: block;
}

#galeria img:hover {
  transform: scale(1.03);
  border: #000 solid 5px;
}

/* ===== TABLA DE DATOS ===== */

table, th {
  border: 2px solid #093649;
  width: 80%;
  margin: auto;
  background-color: #8cdbd6;
  text-align: left;
  font-size: large;
  border-radius: 5px;
}

/* ===== FORMULARIO ===== */

legend {
  font-family: "Press Start 2P", system-ui;
}

fieldset, input {
  font-family: "text";
  font-size: 20px;
  padding: auto;
  margin: 15px;
  border-radius: 15px;
  border: #8cdbd6;
}

 input.boton {
  background-color: #bde3de;
  margin: 20px auto;
  box-shadow: 6px 7px 10px -1px rgba(37,121,138,0.68);
  border: #21556b solid 2px;
  cursor: pointer;
  border-radius: 5px;
  display: flex;
  justify-content: space-between;
  width: 10%;
 }

 input.boton:hover{
  background-color: #a7ccc7;
  border-radius: 5px;
  box-shadow: 4px 5px 8px -1px rgba(37, 121, 138, 0.80);
 }

/* ===== CONTACTO ===== */

#con a {
  color: #000;
}

#con a:hover {
    background-color: #359eb3;
    border-radius: 5px;
}

#con li {
  font-family: "text";
  margin: 15px;
  font-size: 20px;
  margin-left: 50px;
}

/* ===== PIE DE PÁGINA ===== */

.site-footer {
  background-color: #21556b;
  text-align: center;
  padding: 20px;
  font-family: "Opciones";
  color: #bde3de;
}

.site-footer a:visited {
    text-align: center;
    color: #bde3de;
}

.site-footer a:hover{
  color: whitesmoke;
}
```

A continuación veremos ejemplos de algunas cosas utilizadas en este CSS:

Lo primero que destacaremos son los selectores:

```css
#hero figure img {
    height: auto;
    margin: auto;
    display: block;
    width: 80%;
    object-fit: cover;
    border-radius: 10px;
}
```
Como podemos observar aquí, encontramos el id hero y que se espeficica que de ese hero el estilo se pondrán en una imagen dentro de un figure. Decidí hacerlo así ya que es más cómodo seleccionar la imagen del hero.

Un ejemplo de un selector de class sería el siguiente:

```css
.open-menu {
  position: fixed;
  top: 14px;
  left: 14px;
  z-index: 20;
  font-size: 26px;
  cursor: pointer;
  background: none;
  border: none;
  transition: transform 0.3s ease, background-color 0.3s ease;
}
```

A continuación veremos las pseudoclases: 

```css
.side-menu a:hover {
  color: whitesmoke;
}
```
Aquí podemos observar que la pseudoclase sería :hover, que sirve para que cuando el cursos pase por esa zona, el texto se vuelva del color indicado. Lo utilizamos para que se note las opciones al pasar el cursor por ellas. 

Lo siguiente que veremos será un ejemplo de Grid:

```css
#galeria figure {
  display: grid;
  grid-template-rows: repeat(auto-fill, minmax(200px, autofr));
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 20px;
}
```

Primero, se necesita iniciar el grid con "display: grid;" y los siguientes dos líneas sriven para definir las columnas y filas que queremos. El "repeat(auto-fill)" selecciona cuantas filas o columnas colocar dependiedno de cuantas imágenes haya en el figure. El "minmax(200px, autofr/1fr)" sirve para poner un tamaño a las imágenes y el fr sirve para definir el espacio fraccional disponible para cada imágen. Por último, el gap es la separación que hay en cada columna o fila.

Decidí hacerlo así para poder organizar las imágenes de una mejor manera y que quede bien presentado. 

Ahora veremos el uso de box-shadow:

```css
input.boton:hover{
  background-color: #a7ccc7;
  border-radius: 5px;
  box-shadow: 4px 5px 8px -1px rgba(37, 121, 138, 0.80);
 }
```

Como podemos ver, el box-shadow se utiliza en los botones de "Enviar" y "Borrar" de la sección Formulario. Se utiliza para poder destacar bien los botones y para dar una sensación de 3D.

Por último, veremos los estilos de los menús:

```css
.side-menu {
  position: fixed;
  top: 0;
  left: -230px;            
  width: 230px;
  height: 100%;
  background-color: #8cdbd6;
  padding-top: 60px;
  transition: left 0.3s ease;
  z-index: 15;
  font-family: "Opciones";
  display: flex;
  flex-direction: column;
}

.side-menu.active {
  left: 0;   
}

.side-menu ul {
  list-style: none;
  padding: 0;
}

.side-menu a {
  display: block;
  padding: 12px 20px;
  color: #31798c;
  text-decoration: none;
}

.side-menu a:hover {
  color: whitesmoke;
}
```

Como podemos observar aquí, en ".side-menu" sirve para colocar correctamente el menú lateral, es decir, que se ubique a la izquierda de la página y se abra si haces clic en el botón. El resto de detalles son colores para las letras de las opciones combinen con la estética de la página y el ":hover" para cuando se pase el cursor encima cambie el color de las opciones y se note. La fuente "Opciones" sirve para diferenciar del resto de fuentes de la página.

Algo similar ocurre con el menú de la derecha:

```css
.main-nav ul {
  list-style: none;
  display: flex;
  gap: 10px;
}

.main-nav a {
  color: #bde3de;
  padding: 10px;
  font-family: "Opciones";
  text-decoration: none;
  display: flex;
  flex-direction: row;
  justify-content: right;
}
```



### 4.4. Fuentes utilizadas

En este apartado veremos las fuentes que han sido utilizadas.
Primero veremos las fuentes locales:

```css
@font-face {
  font-family: "Título h1";
  src: url("fonts/Digital\ Change\ Demo.ttf") format('truetype');
} 

@font-face {
  font-family: "Opciones";
  src: url("fonts/Blackney-Bold.ttf") format('truetype');
}

@font-face {
  font-family: "text";
  src: url("fonts/Petrona-VariableFont_wght.ttf") format('truetype');
}
```

Para que funcione estas fuentes debemos colocar el @font-face. Dentro de él, debemos ponerle un nombre con font-family y luego indicamos la url del archivo .ttf. Luego, donde queramos colocar está fuente, lo hacemos con el font-family como lo vemos a continuación:

```css
fieldset, input {
  font-family: "text";
  font-size: 20px;
  padding: auto;
  margin: 15px;
  border-radius: 15px;
  border: #8cdbd6;
}
```

Decidí eligir estas tipografías ya que quería que cada texto destacase a diferencia del respecto de tipografías. Por ejemplo: el título tiene una tipografía única, las Opciones solo se usan en los menús y la de text solo se usan en textos que vayan con las etiquetas p.

    Problema sin Solución: Las fuentes utilizadas en el título y en los menús no funcionan y desconozco porque ocurre esto.

A continuación veremos las fuentes online:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap" rel="stylesheet">
```


```css
h2 {
  font-family: "Press Start 2P", system-ui;
  font-weight: 400;
  font-style: normal;
  width: 100%;
  margin: 20px;
}

h3 {
  margin: 15px;
  font-family: "Press Start 2P", system-ui;
  font-weight: 400;
  font-size: 20px;
  width: 100%;
  font-style: normal;
}
```

Para que funcione la fuente online, debemos copiar el enlace que nos proporciona la página Google Fonts y para que se visualice debemos copiar el css que proporciona la página y así se la ponemos, en este caso, a los h2 y h3.

Decidí escoger esta tipografía ya que es una similar a la que se utiliza dentro del videojuego y así el visitante de la página pueda saber cuando empieza una nueva sección. 

### 4.5. Menú lateral: breve explicación

Aquí veremos como funciona el botón del menú lateral brevemente:

```html
<script>
    const sideMenu = document.getElementById("sideMenu");
    const toggleBtn = document.querySelector(".open-menu");
    const toggleIcon = document.getElementById("toggleIcon"); 
    toggleBtn.addEventListener("click", () => {
        sideMenu.classList.toggle("active");
        toggleBtn.classList.toggle("active");
        if (sideMenu.classList.contains("active")) {
            toggleIcon.src = "img/boton-abierto.png"; 
        } else {
            toggleIcon.src = "img/boton.png";
        }
    });
</script>
```

Al pulsar el botón que hay en la página, se abrirá un menú lateral en el cuál puedes elegir dandole clic entre las secciones que hay disponibles y te llevará a ellas. Esto provoca que exista un cambio, el cual consiste de pasar de .open-menu a sideMenu. Este menú puede ser movido con CSS mediante los siguientes ajustes que hay en .side-menu:

```css
.side-menu {
  position: fixed;
  top: 0;
  left: -230px;            
  width: 230px;
  height: 100%;
  background-color: #8cdbd6;
  padding-top: 60px;
  transition: left 0.3s ease;
  z-index: 15;
  font-family: "Opciones";
  display: flex;
  flex-direction: column;
}
```


### 4.6. Conclusión personal



