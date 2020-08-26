# Implementação do List<T>
Faz parte da coleção em C# que implementa uma interface `IList<T>`. Podemos encará-la como a implementação de um array dinâmico, onde o tamanho é ajustado de acordo com a necessidade. Internamente um `array` é utilizado para o armazenamentoe caso haja a necessidade de aumento, uma nova array é criada e os elementos do array antigo são copiados para a nova. Usar `List<T>` promove uma maior economia de memória comparado ao `array`. Vejamos um exemplo de classe usando `List<T>` e seus métodos:

```csharp
public class ListDemo
{
    public static void Main(string[] args)
    {
        List<int> al = new List<int>();
        al.Add(1); // Adiciona 1 no final da lista
        al.Add(2);
        al.Add(3);
        al.Add(4);
        Console.WriteLine("Conteúdo da Lista:");

        al.ForEach(Console.Write);

        Console.WriteLine("\nConteúdo da lista na posição 0:" + al[0]);

        Console.WriteLine("Tamanho da lista:" + al.Count);

        Console.WriteLine("A lista é vazia:" + (al.Count == 0));

        al.RemoveAt(al.Count -1); // Remove o último elemento da lista

        Console.WriteLine("\nTamanho da lista depois do elemento removido;");

        al.Clear(); // Todos os elementos da lista são removidos

        Console.WriteLine("\nA lista está vazia depois do Clear():" + (al.Count == 0));
    }
}

```