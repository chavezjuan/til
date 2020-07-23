# Classe, campos, propriedades e métodos
As classes em C# possuem uma forma específica possuindo Métodos, Propriedades e Campos. Essas estruturas presentes nas classes podem ter uma estrutura muito parecida mas há uma diferença sutil entre elas.
Vamos supor uma classe chamada 'Quarto':
```c#
class Quarto 
{

}
```
Dentro de um quarto temos vários elementos como a cama, janela, ventilador e etc. Esses elementos serão os Campos (*Fields*):
```c#
class Quarto 
{
  public string cama;
  public int janela;
  public int ventilador;
  public bool arcondicionado;
}
```
Por sua vez as Propriedades (*Properties*) são uma forma de definirmos quais valores são válidos e não permitirmos aqueles que não o são. É nessa estrutura que definimos os *Getters* e *Setters*:
```c#
class Quarto 
{
  //Campos
  public string cama;
  public int janela;
  public int ventilador;
  public bool arcondicionado;

  //Propriedades
  public string Cama
  {
      get { return name; }
      set { name = value; }
  }

  public int Janela
  {
      get { return janela; }
      set { janela = value; }
  }

  public bool Ventilador
  {
      get { return ventilador; }
      set { ventilador = value; }
  }

  public bool Arcondicionado
  {
      get { return arcondicionado; }
      set { arcondicionado = value; }
  }
}
```
Como obervado, as Propriedades levam o mesmo nome dos Campos só que a primeira letra é maiúscula. Dentro de cada método `get` e `set` posso definir restrições utilizando estruturas de controle conforme a necessidade. 
<br>
Por fim chegamos aos Métodos (*Methods*). Os Métodos definem como uma instância da classe se comporta. Podemos fazer uma analogia com as "ações" que um "objeto" poderá fazer. No nosso caso, um quarto terá as "ações" de `ligarArcondicionado` e `ligarVentilador`. Assim definimos os seguintes métodos:
```c#
class Quarto 
{
  //Campos
  public string cama;
  public int janela;
  public int ventilador;
  public bool arcondicionado;

  //Propriedades
  public string Cama
  {
      get { return name; }
      set { name = value; }
  }

  public int Janela
  {
      get { return janela; }
      set { janela = value; }
  }

  public bool Ventilador
  {
      get { return ventilador; }
      set { ventilador = value; }
  }

  public bool Arcondicionado
  {
      get { return arcondicionado; }
      set { arcondicionado = value; }
  }
  
  //Métodos
  public bool ligarArcondicionado()
  {
      Arcondicionado = true;
      return Arcondicionado;
  }

  public bool ligarVentilador()
  {
      Ventilador = true;
      return Ventilador;
  }
}
```
Uma vez que definimos as Propriedades, não acessamos diretamente os Campos para definir o seu valor mas através da Propriedade correspondente.
<br>
Podemos observar que as estruturas descritas são muito parecidas entre si, mas cada uma tem um papel bem epecífico dentro de uma classe. Os Construtores são estruturas que podemos definir dentro de uma classe e que possui uma sintaxe bem parecida com o que vimos. Isso iremos abordar em outro tópico.
