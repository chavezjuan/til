# Short-circuit evaluation na atribuição de valores à variáveis

Os operadores lógicos em javascript `&&`, `||` e `!` podem ser utilizados como
uma ferramenta de simplicação na atribuição de um valor a uma dada variável.

```javascript
let nome = username || 'guest'
```
No exemplo acima, caso a variável `username` não for atribuída nenhum valor, será
atribuída a variável `nome` o valor padrão `guest`. Essa estrutura conhecida por 
`short-circuit evaluation` verifica se o primeiro termo da expressão lógica é `true`,
caso contrário é atribuído o segundo termo.
