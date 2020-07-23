# Como configurar o seu repositório local rapidamente e fazer o seu primeiro commit pela linha de comando
Primeiro abra o terminal do seu OS na pasta onde deseja criar seu repositório. Seguindo os seguintes passos vamos da criação até o commit.
## 1. Criar novo repositório
```bash
git init
```
## 2. Adicionar todos os arquivos e diretórios
```bash
git add .
```
## 3. Comitar arquivos e diretórios
```bash
git commit -m "Escreva aqui sua mensagem"
```
## 4. Vinculando repositório local ao remoto
Nesse passo você precisará ter criado um repositório no GitHub e pego o link correspondente.
```bash
git remote add origin https://github.com/seugithub/seurepositorio.git
```
## 5. Primeiro Push
```bash
git push -u origin master
```
Para os próximos `push` só precisa digitar:
```bash
git push
``` 
Pronto. Seu repositório local já se encontra no seu GitHub.