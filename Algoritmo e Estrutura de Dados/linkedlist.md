# LinkedList<T> 
As principais características da Linked List é o fato da exclusão e inclusão poder ser realizada tanto no ínicio quanto no final da lista e a alocação dos dados na memória é dinâmica. Justamente por causa disso a sua performance é inferior a um Array, pois no Array já predefinimos o espaço na memória para alocar o dado. <br>
Dessa forma, um bom uso do Linked List se dá quando não temos certeza da quantidade de dados que iremos armazenar. Vejamos um exemplo da implememtação do Linked List com suas operações e métodos:
```csharp
public class LinkedListDemo
{
    public static void Main(string[] args)
    {
        LinkedList<int> ll = new new LinkedList<int>();
        //Adiciona 10 no início da lista
        ll.AddFirst(10);
        //Adiciona 20 no final da lista
        ll.AddLast(20);
        ll.AddFirst(9);
        ll.AddLast(21);
        ll.AddFirst(8);
        ll.AddLast(22);

        Console.Write("Conteúdo da Linked List: ");
        foreach (int val in ll)
        {
            Console.Write(val + " ");
        }

        ll.RemoveFirst();
        ll.RemoveLast();

        Console.Write("\nConteúdo da Linked List: ");
        foreach (int val in ll)
        {
            Console.Write(val + " ");
        }
    }
}
``` 