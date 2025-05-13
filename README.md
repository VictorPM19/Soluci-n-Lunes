# Soluci-n-Lunes
Código Tecnologías WEB

## Realizar el algoritmo utilizando funciones flecha que me indique el nombre y la edad mayor y menor.

---

```ts
const nombres: string[] = ['Juan', 'Manuel', 'Miguel', 'Victor', 'Hector'];
const edades: number[] = [15, 30, 70, 18, 35];

const personas = nombres.map((nombre, i) => ({ nombre, edad: edades[i] }));

const ordenadas = [...personas].sort((a, b) => a.edad - b.edad);

const menor = ordenadas[0];
const mayor = ordenadas[ordenadas.length - 1];

console.log(`${menor.nombre} es el menor con ${menor.edad} años`);
console.log(`${mayor.nombre} es el mayor con ${mayor.edad} años`);


