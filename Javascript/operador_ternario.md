# Usando operadores ternários para simplificar o código

Podemos substituir a estrutura `if ... else` do javascript fatorando em uma só linha. Por exemplo:

```javascript
const clima = 'chuva'

if (clima === 'chuva') {
  console.log('Levar guarda chuva')
} else {
  console.log('Usar roupas frescas')
}
```
Podemos substituir essa estrutura pelo operador ternário:

```javascript
const clima = 'chuva'

clima === 'chuva' ? console.log('Levar guarda chuva') : console.log('Usar roupas frescas')
```
O primeiro termo do operador após o `?`, é retornado caso a condição anterior ao `?` seja verdadeira `true`, 
caso contrário `false`, é retornado o termo após o `:`.
Dessa forma aumentamos a legibilidade do nosso código.
