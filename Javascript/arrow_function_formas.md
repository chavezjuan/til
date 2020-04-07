# Formas de utilizar a Arrow Function para fatorar o código
Introduzido pelo javascript ES6, a sintaxe arrow function é uma forma curta de
escrever funções no javascript. Tradicionalmente escrevemos funções da seguinte
forma:
```javascript
function rectangleArea(width, height) {

  return width * height
}
```
Caso quisermos escrever na forma de expressão e ao mesmo tempo atribuir a uma variável:
```javascript
const calculateArea = function (width, height) {
 
  return width * height
}
```

Com a arrow function, utilizando a sintaxe `() =>` podemos reescrever a função anterior:
```javascript
const calculateArea = (width, height) => {
  return width * height
}
```
Quanto a quantidade de parâmetros da função, podemos escrever uma arrow function da seguinte
forma:
#### Nenhum parâmetro
```javascript
const functionName = () => {}
```
#### Um parâmetro
```javascript
const functionName = paramOne => {}
```
#### Dois ou mais parâmetros
```javascript
const functionName = (paramOne, paramTwo) => {}
```
Na estruturação de blocos, podemos dispensar o uso das `{}` e do `return` caso o body seja composto de
apenas uma linha. Essa técnica é conhecida como `implicit return`:
```javascript
const sumNumbers = number => {
  return number + number
}
```
Equivalente:
```javascript
const sumNumbers = number => number + number;
```
Dessa forma observamos como a arrow function pode simplificar o nosso código.

