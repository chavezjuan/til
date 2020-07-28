# Interfaces
É um conjunto de ações e valores que descrevem como uma classe pode ser utilizada. Isso já é feito pelo próprio computador quando tentamos declarar um inteiro `int` como `string` por exemplo. Nesse caso é reconhecido a incompatibilidade e um erro é mostrado. Mas para as nossas classes criadas isso não é trivial para o sistema. Precisamos ensiná-lo que a nossa classe espera certos tipos de métodos e propriedades. Para tal utilizamos as Interfaces nos ajudando a previnir diversos erros.
<br>
Como exemplo da implementação, vamos supor que desejemos criar um grupo de requisitos que satisfaça tanto uma loja de automóveis quanto a polícia rodoviária. A polícia necessita das seguintes informações:
* velocidade
* número da placa
* número de rodas
Observamos que são características comuns para ambas. Para tal criaremos uma Interface. Ela somente mostra as propriedades, métodos e ações mas não as definem. Quem irá definir é a classe que implementa essa Interface de acordo com suas regras.
```C#
interface IAutomovel
{
    string NumeroPlaca { get; };
    double Velocidade { get; };
    int Rodas { get; };
}
```
Para identificarmos uma Interface devemos iniciar a palavra pela letra `I`.