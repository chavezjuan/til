# Como rodar o programa .cs no CLI

Primeiro precisa saber qual é o caminho do `csc.exe` no seu computador. Para saber rode o comando no cmd:

```bash
dir /s %WINDIR%\CSC.EXE
```
Uma vez retornado o caminho, copie e cole no cmd acrescentando csc.exe no final como a seguir:

```bash
C:\Windows\Microsoft.NET\Framework64\v4.0.30319\csc.exe
```

Execute e será iniciado o compilador do C#. \nNavegue até a pasta onde você tem o seu arquivo .cs que deseja executar. Digite:

```bash
csc teste.cs
```
Pressione ENTER para compilar. Será gerado um executável na mesma pasta. Para rodar digite:

```bash
teste.exe
```