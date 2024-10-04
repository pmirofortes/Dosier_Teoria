# Titulo del dosier
indice con enlaces

# 1. GITHUB
# 2. MARKDOWN
## 2.1. Titulos
Podemos escribir todo nuestro texto en el documento y ya está pero si lo queremos tener organizado y que facilite la lectura utilizaremos encabezados.

Para crear encabezados utilizaremos "#" 
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
# 4. CSS
# 5. Diseño Responsive