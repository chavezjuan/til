# Erro: Refusing to merge unrelated histories
Esse erro apareceu quando tentei fazer um `push` para meu repositório no GitHub.
<br>
Para solucionar, basta digitar o seguinte comando no seu repositório local:
```bash
git pull origin master --allow-unrelated-histories
```