 Ejercicio: Crea una función en JavaScript/TypeScript que reciba un array de frutas y un objeto `persona` con dos propiedades `nombre` y `edad`. Muestra por consola los siguientes mensajes:

- "Los frutas favoritas son: [lista de frutas]"
- Si la edad de la persona es mayor o igual a 18, muestra "La persona tiene la edad suficiente para conducir". De lo contrario, muestra "La persona no tiene la edad suficiente para conducir".

Explicación:
En este ejercicio nos enfocaremos en trabajar con arrays y objetos. Además, utilizaremos estructuras de control (condicionales) para decidir que mensaje mostrar.

```typescript
function mostrarMensajes(frutas: string[], persona: { nombre: string; edad: number }) {
    // Imprimimos los frutas favoritas
    console.log(`Los frutas favoritas son: ${frutas.join(", ")}`);

    // Comprobamos la edad de la persona y mostramos el mensaje correspondiente
    if (persona.edad >= 18) {
        console.log("La persona tiene la edad suficiente para conducir.");
    } else {
        console.log("La persona no tiene la edad suficiente para conducir.");
    }
}
```

Solución comentada:

```typescript
// Definimos una función que recibe un array de frutas y un objeto persona con dos propiedades: nombre y edad.
function mostrarMensajes(frutas: string[], persona: { nombre: string; edad: number }) {
    // Imprimimos los frutas favoritas
    console.log(`Los frutas favoritas son: ${frutas.join(", ")}`);

    // Comprobamos la edad de la persona y mostramos el mensaje correspondiente
    if (persona.edad >= 18) {
        console.log("La persona tiene la edad suficiente para conducir.");
    } else {
        console.log("La persona no tiene la edad suficiente para conducir.");
    }
}
```

Usa esta función de la siguiente manera:

```javascript
const frutas = ['manzana', 'pera', 'uva', 'naranja'];
const persona = {
  nombre: "Luis",
  edad: 30,
};
mostrarMensajes(frutas, persona);
```

Este código imprimirá los siguientes mensajes:

- "Los frutas favoritas son: manzana, pera, uva, naranja"
- "La persona tiene la edad suficiente para conducir."