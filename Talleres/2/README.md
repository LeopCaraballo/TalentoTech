### Parte 1: Tipos de Datos

```typescript
// Declaración de variables utilizando diferentes tipos de datos
let numero: number = 10;
let cadena: string = 'Hola';
let booleano: boolean = true;
let arreglo: number[] = [1, 2, 3];
let objeto: { nombre: string; edad: number } = { nombre: 'Juan', edad: 25 };

// Uso de tipos de literales para limitar los valores de una variable
let color: 'rojo' | 'verde' | 'azul' = 'rojo';
color = 'verde'; // válido
// color = "amarillo"; // inválido, no es uno de los valores permitidos
```

### Parte 2: Condicionales

```typescript
// Estructuras condicionales (if, else if, else)
let numero: number = 10;

if (numero > 0) {
  console.log('El número es positivo');
} else if (numero < 0) {
  console.log('El número es negativo');
} else {
  console.log('El número es cero');
}
```

### Parte 3: Funciones

```typescript
// Funciones básicas con diferentes tipos de parámetros y tipos de retorno
function sumar(a: number, b: number): number {
  return a + b;
}

function saludar(nombre: string): void {
  console.log('¡Hola, ' + nombre + '!');
}

// Funciones con parámetros opcionales y con valores predeterminados
function calcularArea(base: number, altura: number, tipo: string = 'rectangulo'): number {
  if (tipo === 'rectangulo') {
    return base * altura;
  } else if (tipo === 'triangulo') {
    return (base * altura) / 2;
  }
  return 0;
}
```
