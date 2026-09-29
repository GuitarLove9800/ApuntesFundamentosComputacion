# Tecnológico de Software
## Desarrollo de Software (TSW) | Grupo 1-A

### Glosario General Consolidado: Fundamentos de Programación
**Compendio Integral (Partes 1 y 2)**

> **Materia:** Fundamentos de Computación  
> **Estudiante:** Emmanuel Alexander Poot Vazquez  
> **Fecha:** 24 de septiembre de 2026  

---

### Índice General

| Sección | Página |
| :--- | :---: |
| 1. Introducción y Conceptos Básicos (1 al 6 - Parte 1) | Página 2 |
| 2. Tipos, Operadores y Control de Flujo (7 al 13 - Parte 1) | Página 3 |
| 3. Modularidad, Arreglos y Eventos (14 al 20 - Parte 1) | Página 4 |
| 4. Introducción Parte 2 y Entornos de Software (1 al 6 - Parte 2) | Página 5 |
| 5. Arquitectura y Control de Versiones (7 al 13 - Parte 2) | Página 6 |
| 6. Gestión de Cambios, Asincronía y Tipado (14 al 20 - Parte 2) | Página 7 |
| 7. Conclusiones y Referencias Bibliográficas Completas | Página 8 |

---

## Parte 1: Lógica y Sintaxis Fundamental

*Presenta las bases elementales sobre la estructura y conformación de algoritmos, instrucciones y almacenamiento en memoria.*

### 1. Algoritmo
**Definición:** Serie de instrucciones en lenguaje natural, pseudocódigo o diagramas de flujo para realizar una tarea o resolver un problema. Debe ser preciso, definido, finito y legible.

```javascript
let base = 10;
let altura = 5;
let area = (base * altura) / 2;
console.log(area);
```
*Fuente: CSRC NIST - Algorithm Glossary.*

---

### 2. Programa
**Definición:** Conjunto ordenado de instrucciones redactadas en un lenguaje formal que una computadora interpreta y ejecuta para cumplir un fin computacional determinado.

```javascript
let base = 10;
let altura = 5;
let area = (base * altura) / 2;
console.log(area); // Calcula el área de un triángulo
```
*Fuente: Módulo de Programación Estructurada.*

---

### 3. Código Fuente
**Definición:** Conjunto de líneas legibles por humanos escritas por un desarrollador, las cuales deben someterse a traducción para que la máquina las procese.

```javascript
let edad = 19;
if (edad >= 18) {
    console.log("Mayor de edad");
}
```
*Fuente: MDN Web Docs - JavaScript Language Overview.*

---

### 4. Lenguaje de Programación
**Definición:** Lenguaje formal regido por normas sintácticas y semánticas precisas que faculta la emisión de directivas de cómputo directas.

```python
print("Hola mundo") # Ejemplo ejecutable en Python
```
*Fuente: MDN - JavaScript Language.*

---

### 5. Sintaxis
**Definición:** Reglas estrictas de codificación que rigen la correcta disposición y acoplamiento de variables, palabras reservadas y símbolos.

```javascript
let edad = 19;  // Sintaxis válida
let edad 19;   // Error sintáctico
```
*Fuente: MDN Web Docs - Grammar and Types.*

---

### 6. Variable
**Definición:** Contenedor nombrado en memoria RAM cuyo valor puede reescribirse a lo largo de las distintas etapas del programa.

```javascript
let edad = 19;
edad = 20; // Reasignación de valor en memoria
```
*Fuente: MDN Web Docs - JavaScript Variables.*

---

## Parte 1: Tipos, Operadores y Control de Flujo

### 7. Constante
**Definición:** Identificador vinculado a una posición de memoria cuyo valor es inmutable y no permite reasignaciones tras su inicialización.

```javascript
const PI = 3.1416;
// PI = 5; // Arroja error de tipo TypeError
```
*Fuente: MDN Web Docs - const declaration.*

---

### 8. Tipo de Dato
**Definición:** Clasificación asignada a la información para dictaminar qué valores puede admitir y qué operaciones lógicas/aritméticas se le aplican.

| Tipo | Ejemplo | Representación |
| :--- | :--- | :--- |
| Entero | `19` | Número sin decimales |
| Decimal | `19.5` | Número de coma flotante |
| String | `"Hola"` | Cadena de texto |
| Boolean | `true / false` | Valor lógico binario |

*Fuente: MDN Web Docs - JavaScript data types.*

---

### 9. Operador
**Definición:** Símbolo específico que actúa sobre uno o más operandos para computar un nuevo resultado (aritmético, relacional o booleano).

```javascript
let suma = 5 + 3;
let validacion = (10 > 5) && (2 < 4); // Operadores >, < y &&
```
*Fuente: MDN Web Docs - Expressions and operators.*

---

### 10. Expresión
**Definición:** Segmento ejecutable estructurado por operadores, datos literales y variables que resuelve hacia un único valor concreto.

```javascript
let resultado = 10 * 5; // '10 * 5' es una expresión evaluada a 50
```
*Fuente: MDN Web Docs - Expressions.*

---

### 11. Condicional
**Definición:** Estructura lógica que evalúa una condición booleana para derivar el camino de ejecución del software.

```javascript
if (edad >= 18) {
    console.log("Mayor de edad");
} else {
    console.log("Menor de edad");
}
```
*Fuente: MDN Web Docs - Control flow and error handling.*

---

### 12. Bucle
**Definición:** Ciclo repetitivo de sentencias que se reproduce mientras se satisfaga un predicado lógico o se complete un contador.

```javascript
for (let i = 1; i <= 5; i++) {
    console.log(i); // Genera la salida 1, 2, 3, 4, 5
}
```
*Fuente: MDN Web Docs - Loops and iteration.*

---

### 13. Función
**Definición:** Subrutina modular parametrizable creada para solventar un objetivo determinado, facilitando la no repetición de código.

```javascript
function sumar(a, b) {
    return a + b;
}
```
*Fuente: MDN Web Docs - Functions reference.*

---

## Parte 1: Modularidad, Arreglos y Eventos

### 14. Parámetro
**Definición:** Identificador declarado formalmente en la firma de una función que actúa como receptor del dato que ingresará externamente.

```javascript
function saludar(nombre) { // 'nombre' es el parámetro
    console.log("Hola " + nombre);
}
```
*Fuente: MDN Web Docs - Function parameters.*

---

### 15. Argumento
**Definición:** El dato real, literal o variable suministrado y transferido a la función en el instante preciso de su invocación.

```javascript
saludar("Emmanuel"); // "Emmanuel" funge como argumento
```
*Fuente: MDN Web Docs - Arguments object.*

---

### 16. Retorno
**Definición:** Salida enviada por una función hacia la línea que la llamó por medio de la palabra reservada `return`, concluyendo su ejecución.

```javascript
let total = sumar(5, 3); // Recibe el valor retornado: 8
```
*Fuente: MDN Web Docs - return statement.*

---

### 17. Arreglos (Arrays)
**Definición:** Colección homogénea o heterogénea ordenada de variables a la que se accede por medio de un índice entero de base cero (0).

```javascript
let frutas = ["Manzana", "Plátano", "Naranja"];
console.log(frutas[0]); // Devuelve: Manzana
```
*Fuente: MDN Web Docs - Indexed collections: Array.*

---

### 18. Objeto
**Definición:** Estructura compuesta basada en pares clave-valor capaz de articular atributos estáticos (propiedades) con capacidades dinámicas (métodos).

```javascript
let auto = {
    marca: "Toyota",
    encender: function() { console.log("Motor en marcha"); }
};
```
*Fuente: MDN Web Docs - Working with objects.*

---

### 19. Método
**Definición:** Función asociada orgánicamente a un objeto para realizar operaciones sobre sus estados internos o su contexto.

```javascript
let nombre = "Emmanuel";
console.log(nombre.toUpperCase()); // Método nativo de strings -> EMMANUEL
```
*Fuente: MDN Web Docs - Method definitions.*

---

### 20. Evento
**Definición:** Estímulo o suceso provocado por el usuario o por el sistema ante el cual el software dispara un manejador específico.

```javascript
boton.addEventListener("click", () => {
    console.log("Acción ejecutada por el evento");
});
```
*Fuente: MDN Web Docs - Introduction to events.*

---

## Parte 2: Entornos de Software y Ejecución

*Comprende las utilidades esenciales de construcción de software, ejecución y bibliotecas en entornos profesionales.*

### 1. Compilador
**Definición:** Software de bajo nivel que traduce código fuente a instrucciones de procesador previo a la ejecución, realizando optimizaciones y comprobaciones estructurales.

```cpp
#include <iostream>
int main() {
    std::cout << "Hola mundo";
    return 0;
}
```
*Fuente: IBM - Compiler Concepts.*

---

### 2. Intérprete
**Definición:** Motor computacional que analiza e implementa cada instrucción de código en vivo sin generar un ejecutable previo.

```python
print("Hola mundo") # Procesado de inmediato por el intérprete
```
*Fuente: Python Documentation - Introduction.*

---

### 3. Depurador (Debugger)
**Definición:** Herramienta de auditoría operativa para detener la marcha del código mediante puntos de interrupción y monitorizar memoria en tiempo real.

*Ejemplo: Inspección de variables paso a paso para localizar por qué una función devuelve un resultado no anticipado.*  
*Fuente: Microsoft Learn - Debugging.*

---

### 4. IDE (Integrated Development Environment)
**Definición:** Suite completa de desarrollo que integra editor, terminal, depurador y extensiones en un único espacio unificado.

*Ejemplo: Configuración de VS Code o CLion con compiladores integrados y soporte de extensiones.*  
*Fuente: Microsoft - Visual Studio.*

---

### 5. Editor de Código
**Definición:** Aplicación ligera enfocada primordialmente en la edición ágil de texto plano con soporte de colorimetría sintáctica.

*Ejemplo: Redacción de scripts estructurados dentro de un archivo local 'main.cpp'.*  
*Fuente: Visual Studio Code Documentation.*

---

### 6. Biblioteca (Library)
**Definición:** Conjunto paquetizado de funciones y clases que pueden acoplarse a un desarrollo para ahorrar tiempo de programación.

```python
import math
print(math.sqrt(25)) # Uso de la función prefabricada raíz cuadrada
```
*Fuente: Python Documentation - The Python Standard Library.*

---

## Parte 2: Arquitectura y Control de Versiones

### 7. Framework
**Definición:** Marco de trabajo integral que provee arquitecturas sólidas e invierte el control de la aplicación para crear proyectos escalables.

*Ejemplo: Creación de componentes reutilizables y modulares haciendo uso de la librería React.*  
*Fuente: React Documentation.*

---

### 8. API (Application Programming Interface)
**Definición:** Capa de comunicación protocolar mediante la cual dos componentes o aplicaciones independientes intercambian información.

*Ejemplo: Petición HTTP a un servidor remoto para obtener el estado climático de una región en formato JSON.*  
*Fuente: MDN Web Docs - APIs.*

---

### 9. Repositorio
**Definición:** Directorio centralizado gestionado digitalmente que resguarda ficheros de un proyecto junto a la línea temporal histórica de cambios.

```text
proyecto-cpp/
├── main.cpp
├── README.md
└── .gitignore
```
*Fuente: GitHub Docs - About repositories.*

---

### 10. Control de Versiones
**Definición:** Sistema automatizado para registrar y auditar el historial de cambios en archivos de software a lo largo del tiempo.

*Ejemplo: Revertir un archivo a un estado previo funcional tras experimentar fallas imprevistas.*  
*Fuente: Git Documentation - Getting Started.*

---

### 11. Git
**Definición:** Sistema descentralizado de control de versiones que otorga a cada programador una copia fiel y completa del repositorio.

```bash
git add .
git commit -m "Agrega modulo"
git push origin main
```
*Fuente: Git Official Documentation.*

---

### 12. GitHub
**Definición:** Portal web en la nube que hospeda repositorios remotos gestionados por Git y provee herramientas de colaboración entre pares.

*Ejemplo: Sincronización de tareas académicas en línea para revisión compartida con docentes.*  
*Fuente: GitHub Docs.*

---

### 13. Rama (Branch)
**Definición:** Bifurcación independiente de desarrollo que posibilita ensayar características novedosas sin poner en riesgo la rama principal.

```bash
git branch nueva-funcion
git switch nueva-funcion
```
*Fuente: Git Documentation - Branches.*

---

## Parte 2: Gestión de Cambios, Asincronía y Tipado

### 14. Commit
**Definición:** Instantánea inmutable que guarda el estado de los archivos en Git acompañada de un mensaje descriptivo de la modificación.

```bash
git add main.cpp
git commit -m "Corrige validacion"
```
*Fuente: Git Documentation - Recording Changes.*

---

### 15. Merge
**Definición:** Procedimiento de fusión que acopla los cambios desarrollados en una rama secundaria hacia el tronco principal del proyecto.

```bash
git switch main
git merge nueva-funcion
```
*Fuente: Git Documentation - Basic Branching and Merging.*

---

### 16. Callback
**Definición:** Función transferida como argumento a otra función que se invocará al término de una operación diferida.

```javascript
function terminar() {
    console.log("Operación terminada");
}
setTimeout(terminar, 2000);
```
*Fuente: MDN Web Docs - Callback function.*

---

### 17. Programación Síncrona
**Definición:** Modelo en el cual las sentencias se ejecutan de manera lineal y bloqueante, esperando el término total de cada una.

```javascript
console.log("Primero");
console.log("Segundo");
console.log("Tercero");
```
*Fuente: MDN Web Docs - JavaScript Execution Model.*

---

### 18. Programación Asíncrona
**Definición:** Paradigma no bloqueante donde operaciones prolongadas corren en segundo plano, liberando al hilo principal para seguir trabajando.

```javascript
console.log("Inicio");
setTimeout(() => { console.log("Operación diferida"); }, 2000);
console.log("Fin");
```
*Fuente: MDN Web Docs - Asynchronous JavaScript.*

---

### 19. JavaScript
**Definición:** Lenguaje de scripting de alto nivel, multiparadigma e interpretado para interfaces interactivas y backend (Node.js).

```javascript
let nombre = "GuitarCode";
console.log("Hola " + nombre);
```
*Fuente: MDN Web Docs - JavaScript.*

---

### 20. TypeScript
**Definición:** Superconjunto tipado de JavaScript que añade tipado estático opcional en compilación antes de generar JS puro.

```typescript
let edad: number = 19;
let nombre: string = "GuitarCode";
```
*Fuente: TypeScript Official Documentation.*

---

## Conclusión y Referencias Bibliográficas

### Conclusión General
La asimilación e integración de los 40 conceptos presentados en este compendio sienta una plataforma robusta tanto en el entendimiento de la lógica computacional esencial (variables, estructuras algorítmicas, condicionales, ciclos y modularidad) como en el dominio del entorno de desarrollo contemporáneo (control de versiones con Git, modelos asíncronos y tipado estático). Este conocimiento unificado permite comprender con claridad cómo se conciben, escriben, depuran y distribuyen proyectos de software profesionales.

### Referencias Bibliográficas
1. CSRC NIST. *Algorithm - Glossary*. Computer Security Resource Center.
2. Git Project. *Git Documentation: Getting Started, Branches and Merging*. [https://git-scm.com/doc](https://git-scm.com/doc)
3. GitHub Docs. *About Repositories and Collaborative Development*. [https://docs.github.com/](https://docs.github.com/)
4. IBM Corporation. *Compiler Concepts: AIX 7.2 Documentation*. [https://www.ibm.com/docs/](https://www.ibm.com/docs/)
5. Microsoft Learn. *Visual Studio, VS Code & Debugging Concepts*. [https://learn.microsoft.com/](https://learn.microsoft.com/en-us/visualstudio/)
6. Mozilla Developer Network (MDN). *JavaScript Reference, Grammar, Control Flow, and Web APIs*. [https://developer.mozilla.org/](https://developer.mozilla.org/)
7. Python Software Foundation. *Python Documentation & Standard Library Reference*. [https://docs.python.org/3/](https://docs.python.org/3/)
8. React Community. *React Documentation: Component-Based Architecture*. [https://react.dev/](https://react.dev/)
9. TypeScript Organization. *TypeScript Official Documentation: Handbook*. [https://www.typescriptlang.org/docs/](https://www.typescriptlang.org/docs/)
