## Actividad: Fundamentos de Desarrollo de Software con TypeScript

### 1. Variables:

- **Definición de variable en programación:** En TypeScript, al igual que en otros lenguajes de
  programación, una variable es un contenedor para almacenar datos. Puede contener diferentes tipos
  de datos y su valor puede cambiar durante la ejecución del programa.

- **Declaración de una variable en TypeScript:** En TypeScript, se puede declarar una variable
  utilizando la palabra clave `let` seguida del nombre de la variable y, opcionalmente, su tipo y
  valor inicial:

  ```typescript
  let x: number = 5;
  ```

- **Importancia de asignar un tipo de dato a una variable:** Asignar un tipo de dato a una variable
  en TypeScript es importante porque ayuda al compilador a detectar posibles errores y a ofrecer
  sugerencias durante el desarrollo. Además, mejora la legibilidad del código y facilita su
  mantenimiento.

### 2. Tipos de Datos:

- **Tipos de datos más comunes en TypeScript:** En TypeScript, existen varios tipos de datos que se
  pueden utilizar para definir variables, parámetros de función y otros elementos en el código.

1. **number**: Para representar números, ya sean enteros o de punto flotante.

2. **string**: Para representar datos de texto, como cadenas de caracteres.

3. **boolean**: Para representar valores lógicos, es decir, `true` o `false`.

4. **array**: Para representar una colección de elementos del mismo tipo. Puede definirse con el
   tipo de sus elementos seguido de `[]`.

5. **tuple**: Para representar una colección de elementos heterogéneos. Especifica el tipo de cada
   elemento en una posición fija dentro del array.

6. **enum**: Permite definir un conjunto de constantes con nombre. Cada elemento en el `enum` tiene
   un valor numérico asociado, comenzando desde 0 por defecto.

7. **any**: Se utiliza cuando el tipo de dato de una variable puede ser de cualquier tipo.

8. **void**: Se utiliza principalmente en funciones para indicar que no devuelven ningún valor.

9. **null** y **undefined**: Son subtipos de todos los demás tipos y representan los valores `null`
   y `undefined` respectivamente.

10. **object**: Representa cualquier valor no primitivo. Es el tipo de dato para valores que no son
    números, cadenas, booleanos, null o undefined.

- **Ejemplos de situaciones para cada tipo de dato:**

1. **number**:

   - Ejemplo: Guardar la edad de una persona.

   ```typescript
   let edad: number = 30;
   ```

2. **string**:

   - Ejemplo: Almacenar el nombre de un producto.

   ```typescript
   let nombreProducto: string = 'Camisa';
   ```

3. **boolean**:

   - Ejemplo: Indicar si un producto está disponible en stock.

   ```typescript
   let enStock: boolean = true;
   ```

4. **array**:

   - Ejemplo: Almacenar una lista de nombres de productos.

   ```typescript
   let nombresProductos: string[] = ['Camisa', 'Pantalón', 'Zapatos'];
   ```

5. **tuple**:

   - Ejemplo: Representar las coordenadas de un punto en un plano.

   ```typescript
   let punto: [number, number] = [10, 20];
   ```

6. **enum**:

   - Ejemplo: Definir los días de la semana.

   ```typescript
   enum DiasSemana {
     Lunes, // 0
     Martes, // 1
     Miércoles, // 2
     Jueves, // 3
     Viernes, // 4
     Sábado, // 5
     Domingo, // 6
   }
   let martes: DiasSemana = DiasSemana.Martes; // 1
   ```

7. **any**:

   - Ejemplo: Almacenar datos de un formulario donde los tipos de datos pueden variar.

   ```typescript
   let dato: any = '123';
   dato = 123;
   dato = true;
   ```

8. **void**:

   - Ejemplo: Definir una función que no devuelve ningún valor.

   ```typescript
   function saludar(): void {
     console.log('¡Hola!');
   }
   ```

9. **null** y **undefined**:

   - Ejemplo: Inicializar variables antes de asignarles un valor.

   ```typescript
   let variable1: null = null;
   let variable2: undefined = undefined;
   ```

10. **object**:

- Ejemplo: Representar un objeto con propiedades específicas.

```typescript
let persona: { nombre: string; edad: number } = { nombre: 'Juan', edad: 25 };
```

### 3. Iteradores:

- **Qué son los iteradores y su función en la programación:** En TypeScript, al igual que en otros
  lenguajes, los iteradores son estructuras de control que permiten repetir un bloque de código
  varias veces. Su función es ejecutar instrucciones de forma repetitiva hasta que se cumpla una
  condición.

- **Comparación entre un bucle for y un bucle while:** Las diferencias entre un bucle for y un bucle
  while en TypeScript son similares a otros lenguajes de programación. Un bucle for se utiliza
  cuando se conoce de antemano el número de repeticiones que se deben realizar, mientras que un
  bucle while se utiliza cuando se desconoce el número de repeticiones y se repite hasta que una
  condición se vuelva falsa.

- **Ejemplo de código utilizando un iterador en TypeScript:**

  ```typescript
  // Ejemplo de bucle for
  for (let i = 0; i < 5; i++) {
    console.log(i);
  }

  // Ejemplo de bucle while
  let n = 0;
  while (n < 5) {
    console.log(n);
    n++;
  }
  ```

### 4. Condicionales:

- **Definición de condicionales en programación:** En TypeScript, al igual que en otros lenguajes de
  programación, los condicionales son estructuras de control que permiten tomar decisiones en
  función de si una condición es verdadera o falsa.

- **Diferencia entre una declaración if y una declaración else:**

  - Una declaración `if` se utiliza para ejecutar un bloque de código si una condición es verdadera.
  - Una declaración `else` se utiliza junto con un `if` para ejecutar un bloque de código si la
    condición del `if` es falsa.

- **Programa simple que utiliza condicionales para tomar decisiones en TypeScript:**

  ```typescript
  // Programa que determina si un número es par o impar
  let num: number = 10;

  if (num % 2 === 0) {
    console.log('El número es par');
  } else {
    console.log('El número es impar');
  }
  ```
