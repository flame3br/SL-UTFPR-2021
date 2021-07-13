# Git Assignment

**INDIVIDUAL**

**Entrega**: 15-Jul-21

## Como entregar
Copie o arquivo em um repositorio que seja seu e coloque as respostas nas caixas abaixo

Abra uma issue nesse repositório aqui indicando o link para o arquivo no seu repo.

### Entenda o repositorio
Baixe o arquivo [handson.zip] (handson.zip) e descompacte-o
A pasta handson é um repositório git. Usando a linha de comando, altere o diretório para "handson/"

As caixas vazias
```

```
representam o conteúdo que você precisa preencher e postar em seu repositório privado

1. Descreva qual é a saída dos seguintes comandos
    -  `git branch` 
    -  `git checkout BRANCH_NAME` (USE THE NAME OF AN EXISTING BRANCH)
    -  `git log --decorate`

```
git branch -> exibe as branches existentes
git checkout -> troca branch atual
git log -> exibe commits na branch

```

2. Tente usar `git log --graph --all`. O que acontece?
```
Desenha representação gráfica do histórico de commits da branch

```

3. Use `git diff BRANCH_NAME`  para ver as diferenças de um ramo e do ramo atual.
   Sumarize as diferenças do master e do outro ramo.

```
As classes privadas nos dois são diferentes, um contém a classe A e outro a classe B

```

4. Escreva uma sequencia de comandos para mesclar o ramo não-master no `master`

```
git merge feature-foo
```


5. Escreva um comando (ou sequência) para (i) criar um novo ramo chamado `math` (do` master`)
e (ii) mudar para este ramo

```
git checkout master
git branch math
git checkout math

```
   
6. Edite B.java adicionando o código abaixo ao conteúdo do arquivo
```java
System.out.println("I know math, look:")
System.out.println(2+2)
```

7. Escreva o comando (ou sequencia) para realizar o commit de suas mudanças
```
git add B.java
git commit -m "update B"
```

8. Volte para o branch `master` e mude B.java adicionando o seguinte código-fonte (confirme sua mudança para` master`):
```java
System.out.println("Hello World")
```

9. Escreva uma sequência de comando para mesclar o branch `math` em` master` e descreva o que aconteceu
```
git merge math
As mudanças não commitadas foram detectadas e o merge automático foi cancelado

```
   
10. Escreva um conjunto de comandos para abortar a mesclagem
```
git merge --abort

```
   
11. Agora repita o item 9, mas prossiga com a mesclagem manual (Editando B.java). Todas as funções implementadas são necessárias. Explique o seu procedimento
```
Ambas as alterações foram mantidas, de ambos os commits

```

12. Escreva um comando (ou conjunto de comandos) para prosseguir com a mesclagem e atualizar o branch `master`
```
git add B.java
git commit -m "update B both messages"
git merge math


```



