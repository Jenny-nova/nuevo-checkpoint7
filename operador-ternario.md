# Operador ternario

## ¿Qué es un operador ternario?

Un operador ternario es un operador condicional en JavaScript que evalúa una expresión condicional y devuelve un valor verdadero o falso.

### Sintaxis:

```
conditionalExpression ? truthyValue : falsyValue
```

Según la sintaxis anterior, es `condionalExpression`la expresión que sirve como punto de evaluación, determinando un valor verdadero o falso.

Siguiendo el `?`(signo de interrogación), el valor proporcionado se devuelve en caso de que la expresión se evalúe como verdadera, mientras que el valor que sigue a `:`(dos puntos) se devuelve si la expresión da como resultado un resultado falso a

El `truthyValue` y  `falsyValue` puede ser cualquier cosa en JavaScript. Puede abarcar varias entidades como funciones, valores almacenados en variables, objetos, números, cadenas y más. El operador ternario le otorga la flexibilidad de devolver cualquier valor deseado, ofreciendo versatilidad en su código.

#### **Ejemplo:**

_Estamos creando una plataforma de juegos que solo permite usuarios mayores de 18 años. Diseñaremos una función para comprobar la edad de un usuario. Si son menores de 18 años, se les negará el acceso; De lo contrario, podrán acceder a la plataforma._

```javascript
function canAccessPlatform(age) {
  const shouldAccess = age >= 18 ? true : false;

  return shouldAccess;
}
```

\
A partir del fragmento de código anterior, creamos una función, `canAccessPlatform`que evalúa si un usuario, representado por su `age`parámetro, cumple con el requisito para acceder a la plataforma.

Utiliza un operador ternario para determinar si la edad es 18 o más, asignando `true`si `shouldAccess`se cumple la condición y `false`en caso contrario. Finalmente, devuelve el valor de `shouldAccess`, indicando si el usuario puede acceder a la plataforma o no.

Si la edad es 18 años o más, la expresión se vuelve verdadera, por lo que el operador devuelve verdadero después de `?`. De lo contrario, devuelve falso. Este resultado se guarda en una variable y luego se devuelve desde la función.

Si bien este caso de uso básico simplifica el código y mejora la legibilidad al reemplazar bloques if-else innecesarios, es importante usarlo con moderación para evitar saturar y complicar el código.

### Mejores prácticas al utilizar el operador ternario

El uso eficiente del operador ternario puede mejorar significativamente la legibilidad y la concisión del código.

1. **Manténgalo simple y legible** : escriba expresiones concisas que sean fáciles de entender de un vistazo. Evite anidar demasiados operadores ternarios o escribir condiciones demasiado complejas.
2. **Úselo para asignaciones simples:** los operadores ternarios son ideales para asignaciones simples donde solo hay dos resultados posibles según una condición. Para escenarios más complejos, puede usar `if/else`.
3. **Sepa cuándo usarlo** : utilice el operador ternario cuando necesite realizar una verificación condicional simple y asignar un valor según el resultado. Es particularmente útil para asignar valores predeterminados o determinar el valor de una variable en función de una condición.
4. **Pruebe minuciosamente** : pruebe su código minuciosamente para asegurarse de que el operador ternario se comporta como se espera en diferentes condiciones. Verifique casos extremos y valide la exactitud de los valores asignados.
5. **Evite los ternarios anidados:** si bien es posible encadenar ternarios, el anidamiento excesivo puede generar código difícil de leer. Prefiera claridad y considere su uso `if/else`para condiciones complejas.
6. **Mantenga los ternarios breves:** intente mantener las expresiones ternarias breves y concisas. Los ternarios largos pueden ser difíciles de leer y comprender, lo que genera desafíos de mantenimiento del código.
