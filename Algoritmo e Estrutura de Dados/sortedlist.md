# Como funciona o SortedList<T>
Trata-se de uma estrutura de dados que relaciona `keys` para `values`. Ele é ordenado através das keys em um array. As keys não podem ser repetidas mas os values podem. Ele é uma mistura de um dicionário e um array tradicional, podendo acessar os valores tanto pelo `index` quanto pelo `keys`. Por ser ordenado, a busca pelos valores se dá pelo algoritmo de busca binária.<br>
Um exemplo de suas propriedades e métodos:
```csharp
public class SortedListDemo
{
    public static void Main(string[] args)
    {
        //Definimos uma SortedList com Keys do tipo string e Values do tipo int
        SortedList<string, int> tm = new SortedList<string, int>

        tm["Juan"] = 70;
        tm["Alexandre"] = 23;
        tm["Michel"] = 12;
        tm["Bia"] = 15;

        Console.WriteLine("Quantidade de alunos na classe : " + tm.Count);

        foreach (string key in tm.Keys)
        {
            Console.WriteLine(key + " score marks :" + tm[key]);
        }

        Console.WriteLine("Juan está presente na classe? " + tm.ContainsKey("Juan"));

        Console.WriteLine("Alexandre está presente na classe? " + tm.ContainsKey("Alexandre"));

        Console.WriteLine("Michel está presente na classe? " + tm.ContainsKey("Michel"));

        Console.WriteLine("Bia está presente na classe? " + tm.ContainsKey("Bia"));
    }
}
```
