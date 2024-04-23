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