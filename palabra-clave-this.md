# Palabra clave this

## ¿Qué es la palabra clave `this`en JavaScript?

`this` es una palabra especial que **representa el contexto en el que se ejecuta una función** . Su valor cambia dependiendo de **dónde y cómo se llama una función** .

Un comentario importante es que `this`no es una variable, es una palabra clave, por lo que su valor no se puede cambiar ni reasignar.

### ¿Cuándo se usa?

* Se usa para acceder a propiedades y métodos de un objeto.
* Se usa en los controladores de eventos de HTML para vincularse a los elementos HTML que reciben el evento.
* Se usa en funciones flecha, donde hereda el `this`de la función externa donde se define

### ¿Cómo se comporta?

* Si se llama a `this`por sí mismo, se refiere al objeto de ventana global.

```javascript

function f1() {
  return this;
}

f1() === window; // objeto global
```

* Si se llama a `this`dentro de un método de objeto, se puede usar para acceder a otras propiedades y métodos del mismo objeto.

#### **Ejemplo:**

> ```javascript
> const persona = {
>     nombre: "Laura",
>     saludar: function() {
>     console.log("Hola, soy " + this.nombre);
>     }
> };
> ```

* Si se usa en un detector de eventos, `this`se refiere al elemento DOM que activó el evento

### ¿Por qué es importante entender `this`?

* Para crear objetos y clases correctamente.
* Para trabajar con eventos, formularios, animaciones, etc.
* Para usar correctamente métodos como `.bind()`, `.call()`, y `.apply()`que controlan a qué se refiere `this`.
