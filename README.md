# Titulo del dosier
1. [GITHUB](#1-github "Enlace al apartado de GitHub")
2. [MARKDOWN](#2-markdown "Enlace al apartado de MarkDown")
3. [HTML](#3-html "Enlace al apartado de HTML")
4. [CSS](#4-css "Enlace al apartado de CSS")
5. [DISEÑO RESPONSIVE](#5-diseño-responsive "Enlace al apartado de  Diseño Responsive")

# 1. GITHUB
## 1.1. Instalar Git
Para utilizar Git, primero lo instalaremos. Entrando en este enlace lo descargaremos y en el cmd podremos escribir codigo.

[Git para Windows](https://git-scm.com/download/win)
## 1.2. Crear cuenta en GitHub
1. Visitar [GitHub]([URL](https://github.com/) "enlace a GitHub")
2. Haz clic en "Sign up" (registrarse).
3. Introduce tu nombre de usuario, correo electrónico y una contraseña segura.
4. Completa el proceso de verificación y la configuración de tu cuenta.
5. Una vez registrada, podrás crear repositorios y colaborar en proyectos.
## 1.3. Repositorios
### 1.3.1. Crear repositorio
1. Hacemos click en "Nuevo" en la pagina principal.
2. Hacemos click en "crear repositorio"
### 1.3.2. Clonar repositorio
1. Copiamos la URL del repositorio en GitHub.
2. En la terminal, usarmos el siguiente comando:
```git clone https://github.com/usuario/repo.git```
## 1.4. Codigos Git
 - ```git init```. Se usa para inicializar un repositorio Git en local.
 - ```git branch -M "rama"```. Se usa para cambiar a otras ramas.
 - ```git branch```. Se usa para listar las ramas del repositorio.
 - ```git add "archivo.txt"```. Se usa para añadir agregar los archivos al area intermedia antes de hacer el commit. Podemos escribir el nombre de los archivos o usar "." para añadir todos los archivos.
 - ```git commit -m "Mensaje del commit"```. Se usa para guardar los cambios del area intermedia en el commit para posteriormente subirlo. 
 - ```git push origin main```. Se usa para enviar el commit a la rama "origin" desde "main" y subirlo a github.
 - ```git remote add origin https://github.com/usuario/repo.git```. Se usa para clonar un repositorio remoto a nuestro local.

[Enlace al encabezado](#titulo-del-dosier "Enlace al encabezado")

# 2. MARKDOWN
## 2.1. Titulos
Podemos escribir todo nuestro texto en el documento y ya está pero si lo queremos tener organizado y que facilite la lectura utilizaremos encabezados.

Para crear encabezados utilizaremos "#" y pondremos tantos "#" como niveles de titulo querramos poner.
```
# Titulo de nivel 1
## Titulo de nivel 2
### Titulo de nivel 3
```

## 2.2. **Negrita** y _cursiva_
Para escribir un texto en _cursiva_ utilizaremos uno de estos operadores al inicio y al final del texto ( _ o *) y para la **negrita** utilizaremos 2:
```
Texto en **negrita**

Texto en _cursiva_
```

## 2.3. Listas
Para crear indices o listas se hará igual que en cualquier procesador de texto, colocando el numero y luego el titulo o texto que querramos, por ejemplo:

1. Primer elemento
2. Segundo elemento
3. Tercer elemento   

- Primer elemento
* Segundo elemento
+ Tercer elemento

## 2.4. Mostrar código
Para mostrar un codigo utilizaremos 3 veces " ` " al comienzo y al final de este modo:
```
    ```
    Aqui escribiremos nuestro codigo para mostrarlo en la web

    ```
```
A continuación hay un ejemplo de uso:

```
function calcularPromedio(numeros) {
    let suma = 0;
    for (let i = 0; i < numeros.length; i++) {
        suma += numeros[i];
    }
    return suma / numeros.length;
}

const notas = [8, 7.5, 9, 10, 6];
console.log("El promedio es: " + calcularPromedio(notas));
```

## 2.5. Enlaces e imagenes
### Enlaces
Aplicar un enlace en nuestra web es tan facil como  utlizar este operador (previamente habremos copiado el enlace a la web):
```
[TextoClicable](URL "Titulo opcional")
```
[Wikipedia sobre Spiderman](https://es.wikipedia.org/wiki/Spider-Man#:~:text=Spider-Man,%20traducido%20en%20ocasiones%20como#:~:text=Spider-Man,%20traducido%20en%20ocasiones%20como "Wiki spidey")


### Imagenes 
Colocar imagenes en nuestra pagina es igual de sencillo que los enlaces pero antes habremos descargado la imagen y ubicado en nuestro repositorio:

```
![TextoAlternativo](UbicacionDeLaImagen "Titulo Opcional")
```
![Gif Spidermna](spiderman-animated-gif.gif "Gif Spiderman")



## 2.6. Tablas
Para la creación de tablas primero haremos los títulos:
```
|Título 1|Título 2|Título 3|
```
Luego definiremos los caracteres para una columna (el número de guiones que hay):
```
|Título 1|Título 2|Título 3|
|------------|:-------:|----------------:|

```
(los : indican la alineacion que tiene la columna, a la izquierda, a la derecha o centrada.) Por ultimo escribiremos los datos en las celdas que necesitemos
```
|Título 1|Título 2|Título 3|
|------------|:-------:|----------------:|
|Perros|1200|Adoptados|
|Gatos|700|Refugio|
|Peces|22|Comprados|

```
Así quedaría nuestra tabla:

|Título 1|Título 2|Título 3|
|------------|:-------:|----------------:|
|Perros|1200|Adoptados|
|Gatos|700|Refugio|
|Peces|22|Comprados|

Esta tabla por defecto viene con el estilo de zebra stripes que nos ayuda a la lectura de tablas.

[Enlace al encabezado](#titulo-del-dosier "Enlace al encabezado")
# 3. HTML
## 3.1. Introducción
Tim Berners-Lee creó HTML (HyperText Markup Language), es el lenguaje de marcas mas importante de internet, sin HTML no se veria nada en el navegador.

HTML define la estructura y contenido (imagenes, listas, enlaces...) mediante _etiquetas_, ademas, este lenguaje es muy facil de entender e interpretar, por eso es tan usado en las webs, lo que hace es formatear un texto plano para darle estructura. Tambien le da apariencia a un texto usando [css](#4-css "Enlace al apartado de CSS").

### 3.1.1. Etiquetas
HTML está estructurado a base de etiquetas:
la etiqueta de apertura indica el inicio de un bloque ```<p>``` y las de cierre indican el final de un bloque pero no siempre se cierran ```</p>```.
### 3.1.2. Atributos
Los elementos pueden tener atributos que dan informacion extra a una etiqueta, por ejemplo ``` <img src="direccion de la imagen">"Texto de la imagen" </img> ``` esta etiqueta indica donde se encuentra la imagen y proporciona un texto a la imagen.
## 3.2. Estructura básica de HTML
Un documento HTML está estructurado de esta manera:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```
- ```<!DOCTYPE html>```: Define que el documento es HTML5.
- ```<html></html>```: Contenedor principal del documento.
- ```<head></head>```: Contiene informacion que no se muestra en la web.
  - ```<meta></meta>```: Define metadatos como la codificación de caracteres y la configuración de la visualización.
  - ```<title></title>```: Establece el titulo de tu pagina que aparece en las pestañas del navegador.
- ```<body></body>```: Muestra el contenido visible.

## 3.3. Etiquetas básicas de html
Las etiquetas se clasifican en 2 tipos:
### Elementos de bloque
Es un elemento que necesita una linea nueva para ejecutarse.

`<h1>`-`<h6>`, `<p></p>`, `<ul>`, `<ol>`, `<li>`

### Elementos de línea
Es un elemneto que se encuentra en la misma linea, es decir que se ejecuta detras de otro bloque.

`<a>`, `<strong>`, `<em>`

Tambien podemos añadir comentarios para despues leer el codigo y saber lo que escribimos en el pasado.  ``` <!--ejemplo de comentario--> ``` 

### Rutas
En HTML se utilizan rutas para referenciar imagenes o enlaces. Se puede hacer de forma relativa o absoluta:
- Ruta absoluta. Especifica la ubicacion completa del archivo en la web, es util cuando el archivo se encuentra en un servidor diferente o en una ubicacion especifica de la web. Por ejemplo: ```<img src="https.//www.example.com/images/logo.png" alt="Logo de Ejemplo">```
- Ruta relativa. Especifica la ubicación en relación con el archivo actual. Es útil cuando los archivos están dentro del mismo dominio o estructura de carpetas.

### Imagenes
Para insertar imagenes usamos la etiqueta ```<img>``` con el atributo **```src```** que especifica laruta de la imagen. Tambien podemos añadir **```alt```**  para proporcionar un texto alternativo y **```width```**, **```height```** para darle tamaño a la imagen. Ejemplo:
```
<img src="logo.png" alt="Logo de la página" width="100" height="100">
```


### Enlaces
Para insertar links usamos la etiqueta ```<a><\a>``` que tiene el atrbuto **```href```** que indica la direccion del enlace. Ejemplo:
```
<a href="https://www.ejemplo.com">Visitar Ejemplo</a>
```

## 3.4. Validación de HTML
Es el proceso de verificar que el codigo de HTML cumple con los estandares establecidos por el World Wide Web Consortium. La Validación ayuda a detectar fallos.

[W3C](https://validator.w3.org "Validador de HTML W3C")

## 3.5. Formularios
En HTML, los formularios son una herramienta fundamental para recopilar datos del usuario y enviarlos para su procesamiento (por ejemplo, a un servidor o base de datos).

### 3.5.1. Etiquetas principales para formularios

```<form>```: Se utiliza para definir un formulario. Acepta atributos como:

  - action: Especifica la URL donde se enviarán los datos.
  - method: Define el método HTTP para enviar los datos (GET o POST).

```<input>```: Se emplea para recibir datos del usuario. Atributos comunes:

  - type: Define el tipo de entrada. Ejemplos:
    - text: Campo de texto simple.
    - password: Oculta el texto introducido (contraseñas).
    - radio: Botón de selección única entre varias opciones.
    - checkbox: Casilla de verificación.
    - placeholder: Muestra un texto informativo dentro del campo cuando está vacío.
    - submit: Para enviar el formulario.

```<textarea>```: Define un área de texto multilínea. Atributos importantes:
  - rows: Número de filas visibles. 
  - cols: Número de columnas visibles.
  - placeholder: Texto informativo cuando está vacío.

```<select>```: define el contenedor de un menú desplegable.

```<option>```: define cada opción del menú. Puede incluir el atributo ```disabled``` para deshabilitar opciones.

```<fieldset>```: agrupa elementos relacionados en un formulario, creando un bloque lógico.

```<legend>```: proporciona un título para el grupo.

```<button>```: Define un botón interactivo, generalmente para enviar el formulario.


```
    <form action = "recepcion.png" method = "GET">   
        <label for = "nombre">Nombre :</label>
        <input type = "text" id ="nombre" name ="nombre" placeholder = "Introduce tu nombre"><br><br>
        <label for = "password" >Contraseña :</label>
        <input type = "password" id ="password" name ="password" placeholder ="Introduce tu contraseña"><br><br>
        <fieldset>
            <legend>Idioma</legend>
            <input type = "radio" id="idioma" name = "idioma" value = "castellano">
            <label for = "castellano">Castellano</label>
            <input type = "radio" id="idioma" name = "idioma" value = "catalan">
            <label for = "catalan">Catalán</label>
            <input type = "radio" id="idioma" name = "idioma" value = "chino">
            <label for = "chino">Chino</label>
        </fieldset>
        <fieldset>
            <legend>Nacionalidad</legend>
            <input type = "checkbox" name = "nacionalidad" value = "espanola">
            <label for = "espanola">Española</label>
            <input type = "checkbox" name = "nacionalidad" value = "alemana">
            <label for = "alemana">Alemana</label>
            <input type = "checkbox" name = "nacionalidad" value = "andorrana">
            <label for = "andorrana">Andorrana</label>
        </fieldset>
        <legend></legend>
        <label for="observaciones"> Observaciones</label>
        <textarea name ="observaciones " id="observaciones" cols="80" rows="4" placeholder="Introduce tu comentario"></textarea>
        <label for="ciudad">Ciudad</label>
        <select id="ciudad" name="ciudad">
            <option value=""disabled>Seleccione una ciudad</option>
            <option value="Barcelona">Barcelona</option>
            <option value="Madrid">Madrid</option>
            <option value="Valencia ">Valencia</option>
            <option value="Sevilla">Sevilla</option>
            <option value="Murcia">Murcia</option>
        </select>
        <br><br>
        <button type="submit"> Enviar datos</button>
    </form>

```

![Ejemplo form](/ejemplo_form.png "ejemplo form")

[Enlace al encabezado](#titulo-del-dosier "Enlace al encabezado")
# 4. CSS

## 4.1. Introducción
CSS (Cascading Style Sheets) es un lenguaje de diseño utilizado para controlar la presentación y el estilo de documentos HTML. Permite separar el contenido de su presentación visual.

## 4.2. Formas de aplicar CSS

### 4.2.1. CSS en línea
Se aplica directamente a un elemento HTML usando el atributo `style`:
```
<p style="color: blue;">Texto azul</p>
```

### 4.2.2. CSS interno
Se define dentro de la etiqueta `<style>` en el `<head>` del documento HTML:
```
<head>
  <style>
    body {
      background-color: #f0f0f0;
      font-family: Arial, sans-serif;
    }
    p {
      color: green;
    }
  </style>
</head>
```

### 4.2.3. CSS externo
Se escribe en un archivo separado con extensión `.css` y se enlaza al HTML:
```
<head>
  <link rel="stylesheet" href="estilos.css">
</head>
```

## 4.3. Selectores CSS

### 4.3.1. Etiqueta
Selecciona elementos por su etiqueta HTML:
```
p { 
    font-size: 16px; 
}
```

### 4.3.2. Clase
Selecciona elementos con un atributo `class` utilizando ".clase":
```
.destacado { 
    background-color: yellow; 
}
```

### 4.3.3. ID
Selecciona un elemento con un atributo `id` específico:
```
#header { 
    height: 100px; 
}
```

### 4.3.4. Universal
Selecciona todos los elementos usando el * :
```
* { 
    margin: 0; padding: 0; 
}
```

## 4.4. Propiedades básicas en CSS

### 4.4.1. Colores y fondo
`color: #FF0000;` (Color de texto)  
`background-color: blue;` (Color de fondo)  
`background-image: url('imagen.jpg');` (Asigna una imagen de fondo)

Los colores se basan en combinaciones RGB y HEX, puedes consultarlas en este enlace y asi recibir el codigo del color que tu quieras: [RGB Colores](https://htmlcolorcodes.com/es/ "Titulo opcional")

### 4.4.2. Texto
`font-family: Arial, sans-serif;`  
`font-size: 18px;`  
`font-weight: bold;`  
`text-align: center;`  
`line-height: 1.5;`

### 4.4.3. Tamaños y márgenes
`width: 300px;` (Ancho)  
`height: 200px;` (Alto)  
`margin: 10px;` (Margen exterior)  
`padding: 20px;` (Relleno interior)  
`border: 1px solid black;` (Borde)

### 4.4.4. Posicionamiento
`position: relative;` (relative | absolute | fixed)  
`top: 20px;`  
`left: 50px;`  
`right: 0;`  
`bottom: 0;`

#### 4.4.4.1. Tipos de posicionamiento:
- **absolute**: Se posiciona respecto al ancestro posicionado más cercano
- **relative**: Se posiciona respecto a su posición normal
- **fixed**: Se posiciona respecto a la ventana del navegador

### 4.5.3. Distribución de Hijos
En CSS, los "hijos" se refieren a elementos HTML que están directamente contenidos dentro de otros elementos. Existen varias formas de seleccionarlos y estilizarlos:
- Selector directo >
```css
/* Selecciona solo los <li> que son hijos DIRECTOS de <ul> */
ul > li {
  color: red;
}
```

- Selector descendiente

```css
/* Selecciona TODOS los <p> dentro de <div>, sin importar el nivel */
div p {
  font-weight: bold;
}

```
- Combinación con pseudo clases

```css
/* Primer hijo directo de un contenedor */
.container > :first-child {
  font-size: 1.2em;
}

/* Ultimo hijo directo de un contenedor */
.container > :last-child {
  font-size: 1.2em;
}

/* Cada tercer hijo en una lista */
ul > li:nth-child(3n) {
  background: lightgray;
}
```



[Enlace al encabezado](#titulo-del-dosier "Enlace al encabezado")
# 5. DISEÑO RESPONSIVE
## 5.1. Conceptos Clave
El **Diseño Responsive** (RWD) permite que las páginas web se adapten automáticamente a diferentes dispositivos mediante:

- **Media Queries**: Reglas CSS condicionales
- **Layouts flexibles**: Flexbox/Grid
- **Imágenes escalables**

## 5.2. Media Queries
```css
.container { width: 100%; }

/* Tablet */
@media (min-width: 768px) {
  .container { width: 750px; }
}

/* Desktop */
@media (min-width: 1024px) {
  .container { width: 980px; }
}
```
## 5.3. Flexbox

### 5.3.1. Conceptos Básicos
Flexbox es un **modelo de layout CSS** para diseñar estructuras flexibles y responsivas con un solo eje (fila o columna).

```css
.container {
  display: flex; 
}
```
- Direction
```css
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```
Esto indica si se muestra en fila/fila inversa o en columna/columna inversa. Por defecto, viene con row.
![Flex-direction](./flex-direction.svg " Flex-direction")

- Align-items
```css
.container {
  align-items: stretch;    /* Estira para llenar contenedor */
  align-items: flex-start; /* Arriba */
  align-items: flex-end;   /* Abajo */
  align-items: center;     /* Centrado vertical */
  align-items: baseline;   /* Alineado por línea base */
}
```
- Justify Content
```css
.container {
  justify-content: flex-start;    /* Al inicio (izquierda) */
  justify-content: flex-end;      /* Al final (derecha) */
  justify-content: center;        /* Centrado */
  justify-content: space-between; /* Espacio entre ítems */
  justify-content: space-around;  /* Espacio alrededor */
  justify-content: space-evenly;  /* Espacio uniforme */
}
```

[Enlace al encabezado](#titulo-del-dosier "Enlace al encabezado")
