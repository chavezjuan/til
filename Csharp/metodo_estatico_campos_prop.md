# Campos e propriedades estáticos
Utilizamos um membro do tipo estático quando queremos relacionar uma informação própria da classe. Esse tipo de informação não pode estar associada e acessível a uma instância dessa classe pois não é própria dela. 
<br>
Como exemplo, podemos supor uma classe chamada `Floresta` que possui como campos `idade`, `bioma` e `florestasCriadas`. O último campo trata-se de uma característica própria da classe `Floresta` e não apenas a uma instância. Dessa forma ela é uma boa candidata a um membro estático:
```c#
class Floresta
{
    public int idade;
    private string bioma;
    private static int florestasCriadas;

    
    public int Idade
    {
        get { return idade; }
        private set { idade = value }
    }

    public string Bioma
    {
        get { return bioma; }
        set { bioma = value; }
    }
    
    public static int FlorestasCriadas
    {
        get { return florestasCriadas; }
        private set { florestasCriadas = value; }
    }
}
```
Caso tente acessar `florestasCriadas` através de uma instância da classe dará erro, pois tipos estáticos são acessíveis apenas pela Classe associada.