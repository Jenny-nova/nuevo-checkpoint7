# Condicionales

### ¿Qué son las condicionales en JavaScript?

Las condicionales en JavaScript son estructuras de control que permiten ejecutar diferentes bloques de código según si se cumple o no una determinada condición. Estas estructuras son fundamentales en la programación, ya que permiten que el programa tome decisiones y se comporte de manera dinámica en función de las entradas o el estado del programa.

#### Sintaxis de las condicionales

**1. Sentencia`if`**

La forma más básica de una condicional es la sentencia if. Su sintaxis es la siguiente:

> ```javascript
> let edad = 18;
> if (edad >= 18) {
> console.log("Eres mayor de edad.");
> }
> ```

**2. Sentencia`if...else`**

Si deseas ejecutar un bloque de código cuando la condición es falsa, puedes usar else:

> ```javascript
> let temperatura = 30;
> if (temperatura > 25) {
> console.log("Hace calor.");
> } else {
> console.log("Hace fresco.");
> }
> ```

**3. Oración`else if`**

Para evaluar múltiples condiciones, puedes encadenar varias sentencias `if`con `else if`:

> ```javascript
> let nota = 85;
> if (nota >= 90) {
> console.log("A");
> } else if (nota >= 80) {
> console.log("B");
> } else if (nota >= 70) {
> console.log("C");
> } else {
> console.log("D");
> }
> ```

\
Existen también **los operadores lógicos** , donde puedes combinar múltiples condiciones usando operadores lógicos como `&&`(y) y `||`(o).

**Por ejemplo:**

> ```javascript
> if (condición 1 && condición 2) {
> // Se ejecuta si ambas condiciones son verdaderas
> } else if (condición 1 || condición 2) {
> // Se ejecuta si al menos una de las condiciones es verdadera
> }
> ```

#### ¿Para qué se utilizan?

Las condicionales se utilizan para:

* Tomar decisiones: Permiten que el programa ejecute diferentes basados ​​en acciones específicas.
* Controlar el flujo del programa: Ayudan a dirigir la ejecución del código, permitiendo que ciertas partes se ejecuten solo cuando se cumplen ciertas condiciones.
* Validar datos: Se pueden usar para verificar si los datos ingresados ​​por el usuario cumplen con ciertos criterios antes de proceder con otras operaciones.

#### Beneficios de las condicionales

* **Flexibilidad** : Permiten que el código se adapte a diferentes situaciones y entradas.
* **Legibilidad** : Hacen que el código sea más fácil de entender al mostrar claramente las decisiones que se están tomando.
* **Mantenimiento** : Facilitan la modificación del comportamiento del programa sin necesidad de reescribir grandes secciones de código.
