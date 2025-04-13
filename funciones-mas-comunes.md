# Funciones más comunes

### ¿Cuáles son las tres funciones más comunes de `String`JavaScript?

Los  **cuerdas** son cadenas de texto como `"Hola mundo"`. En JavaScript, se representan entre comillas ( `"`, `'`, o `` ` ``).

#### 1. `.length`– Saber cuántos caracteres tiene una cadena

> ```javascript
> let saludo = "Hola";
> console.log(saludo.length); // 4
> ```

Esto es útil, por ejemplo, para verificar si el usuario escribió suficiente texto en un formulario.

#### 2. `.toUpperCase()`y `.toLowerCase()`– Cambiar mayúsculas/minúsculas



* `.toUpperCase()`convierte todo a MAYÚSCULAS.
* `.toLowerCase()`convierte todo a minúsculas.

Se usa combinado para comparar textos sin importar las mayúsculas.

#### 3.- `.includes()`Verificar si un texto contiene otro

Devuelve `true`si la cadena contiene el texto especificado.

> ```javascript
> let frase = "Me gusta programar";
> console.log(frase.includes("programar")); // true
> console.log(frase.includes("dormir")); // false
> ```

Es ideal para validar contraseñas, buscar palabras o aplicar filtros en listas de texto.
