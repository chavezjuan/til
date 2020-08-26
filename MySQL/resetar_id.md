# Como resetar a contagem do ID em uma tabela habilitada para auto incremento

No banco de dados desejado, faça a seguinte Query após deletar as informações que deseja:

```SQL
DBCC CHECKIDENT ('VesselName', RESEED, 0);
GO
```
Onde no exemplo utilizei uma tabela chamada `VesselName`. No seu caso basta substituir pelo nome da tabela desejada.