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
*Figura 1: Código de JavaScript para cálculos de notas*


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
*Figura 2: Ejemplo de aplicar imágenes*


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
En HTML podemos implementar fromularios para rellenar datos y enviarlos (si queremos a una base de datos)
### 3.5.1. Etiquetas de formularios
```<form>```

```<input> ```

```<textarea> ``` 

```<label> ```

```<select> ```

```<option> ```

```<fieldset> ```

```<legend> ```

```<button> ```

Ejemplo de un formulario en HTML:
```
<form action = "recepcion.png" method = "GET">   
        <label for = "nombre">Nombre :</label>
        <input type = "text" id ="nombre" name ="nombre" placeholder ="Introduce tu nombre"><br><br>
       
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


# 4. CSS
# 5. Diseño Responsive