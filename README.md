# Arrays

- una array es una zona de almacenamiento continuo, donde se pueden introducir varios valores cada uno de ellos ubicado por la poscicion que ocupa en el array.

- También son denominados arreglos o vectores, y cuando son de dos dimensiones son llamados matrices.

- Los arrays nos brindan la capacidad de almacenar una coleccion de elementos y accedar a ellos de manera individual.

- Cada elemento se identifica mediante su poscición en el array denominada **indice** y estos indices son siempre secuenciales.

- en javascript son altamente flexibles en terminos de los diferentes tipos de datos que podemos almacenar en cada poscición del array.

## Crear un array

1. Declarando un array con elementos en linea

```javascript
let miArray = [1, 2, 3,];
console.log(miArray);
```

2. Declarando un array con la sintaxis **new Array()**

```javascript
let miArray = new Array(1, 2, 3);
console.log(miArray);
```

3. Declarando un array con un tamaño específico utilizando la sintaxis **new Array** y asignar valores después:

```javascript
let miArray = new Array(3);
miArray[0] = 1;
miArray[1] = 2;
miArray[2] = 3;
console.log(miArray);
```

4. Declarando un array con elementos de diferentes tipos de datos 

```javascript
let miArray4 = [1, "dos", true, {nombre: "juan", edad: 30}];
console.log(miArray4);
```

## Accediendo a la informacion de un array

### Propiedad length
- Devuelve la cantidad de elementos del array

### operador [pos]
- Permite acceder para leeer o modificar el elemento pos del array

### Metodo at(pos)
- Devuelve el elemento de la poscicion pos. El parametro admite valores negativos, lo que significa que empiezan a contar el final del array.

```javascript
const letters = ["A", "B", "C"];
console.log(letters.length);
console.log(letterts[2]);
console.log(letterts[5]);
```

## Añadir o eliminar elemetos
- push(ele1, ele2): añade uno o mas elementos al final del array. Devuelve el tamaño del array.

```javascript
let miArray = [1, 2, 3];
miArray.push(4); // Agrega el numero 4 al final del array
console.log(miArray);
```

- pop(): Devueve el ultimo elemnto del array y lo elimina

```javascript
let miArray = [1, 2, 3];
miArray.pop(); // elimina el ultimo elemento del array
console.log(miArray);
```

- unshift(ele1, ele2): añade uno o varios elementos al inicio, dvolviendo el tamaño del arrray despues de añadidos

```javascript
let miArray = [1, 2, 3];
miArray.unshift(0); // agrega el elemento 0 al inico del array
console.log(miArray);
```

- shift(): devuelve el primer elemento del array y lo elimina


```javascript
let miArray = [1, 2, 3];
miArray.shift(); // elimina el primer elemento del array
console.log(miArray);
```


- concat(ele1, ele2): concatena dos arrays


```javascript
let miArray = [1, 2, 3];
let miOtroArray = [4, 5];
let nuevoArray = miArray.concat(miOtroArray);
console.log(miArray);
console.log(miOtroArray);
console.log(nuevoArray);
```


- split(separador): a partir de una cadena, crear un array dividiendo dicha cadena en elementos delimitados por separador


```javascript
let miString = "hola, ¿como estas?";
lit miArray = miString.split(" ");
console.log(miArray);
```


- join(separador): a partir de un array, crea una cadena separando cada elemento con el separador


```javascript
let miArray = ["Hola,", "¿como", "estas?"];
let miString = miArray.join(" ");
console.log(miString);
```

## Busqueda de elementos en un array
- includes(elemento): devueve truo o false si el elemento existe o no dentro del array
- indexOf(elemento): devuelve la poscicion de la primera aparicion del elemento, si no existe devuelve -1.
- lastIndexOf(elemennto): devuelve la posicion de la ultima aparicion del elemento, si no existe devuelve -1.

## modificar el array o crear fragmentos
- slice(inicio, fin): devueve un array con los elementos desde la poscicion inicio hasta la poscicicon fin ambos excluidos.

## ordear elementos de un array
- reverse(): invierte el orden de los elementos del array
- sort(): ordena el array alfabeticamente
- sort(criterio): orde el array con el criterio determinado por la funcion criterio.

## Borrar elementos de un array
- se puede borrar el contenido de un elemento de un array poniendo su valor a null o asignando una cadena vacia " ".
- para eliminar completamente un elemento del array se utiliza el operador delete

## recorrido de un array
1. Recorrer con un bucle clasico pasando por todos los elementos.
```javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(i=0<dias.ength;i++)
{
    console.log(dias[i]);
}
```

2. Recorrer con un while pasando por todos los elementos.
```javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
var i = 0;
while(i<dias.ength)
{
    console.log(dias[i]);
    i++;
}
```

3. usando la sentenca for..in.
```javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(let index in dias)
{
    console.log(dias[index]);
}
```

## Arrays multidimensionales
```javascript
const matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
```

- Recorrer una matriz utilizando bucles anidados

```javascript
var dias = ["lunes", "martes", "miercoles", "jueves", "viernes", "sabado", "domingo"];
for(i=0<matriz.ength;i++)
{
    for(let j=0;matriz[i].)length; j++
    {
        console.log(matriz[i][j]);
    }
}
```

# Ejercicios

1. Dada una lista de numeros separados por coma, calcular la suma, el mayor, el menor y la media de todos

2. Introducir dos cadenas con elementos separados por coma, y con un boton concatenar las dos cadenas y mostrarlas en pantalla.

3. introducir uno a uno los elementos en un array a traves de un boton. con otro boton se va eliminando el ultimo elemento. siempre que se pulse alguno de los botones debe mostrar el contenido del array

4. Introducir un conjunto de números separados por comas. Cuando se pulsa el botón "Pares" cargar una tabla con los números introducidos y luego crear otra que solo incluya los números pares y mostrarla.