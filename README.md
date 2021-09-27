# Primeiro trabalho prático de Tópicos Especiais em Programação I
**Leonardo F. E. Albergaria e Rafael de O. Cozer
DI/UFES**

## Visão Geral
> O projeto visa simular a interface básica de um  serviço de streaming de videos, implementando funções básicas como cadastro, login, procura de filmes, etc. O código foi elaborado utilizando-se diversas TAD's, atribuindo cada funcionalidade do sistema à uma biblioteca específica. 
> Nos tópicos a seguir, um pouco de cada uma dessas funcionalidades implementadas, seguindo a linha de raciocínio utilizada.


### 1. Menus

> Nessa biblioteca implementou-se a impressão e uso dos menus de interação do programa, como os menus login, principal e perfil. Foi a base inicial do programa, à fim de conectar as outras funcionalidades e poder rodar os primeiros testes. 


### 2. Usuario

> Em seguida, criou-se a biblioteca de usuários, onde implementou-se as funcionalidades necessárias para que o arquivo de usuários fosse acessado. Após a implementação do menu, essa foi a biblioteca mais importante, pois a partir daqui poderia-se fazer alterações aos perfis de usuários relacionadas ao login, cadastro, exclusão de conta, histórico pessoal, etc. 

### 3. Filmes

> Nessa biblioteca, implementou-se as funções necessárias por ler e imprimir o arquivo de filmes, o que seria a terceira prioridade na linha de racíocinio para eleaboração desse projeto. Aqui, permite-se ao usuário assistir e procurar à um filme, bem como ter acesso aos metadados dos filmes e, após assistir, poder atribuir uma nota ao filme assistido. 


### 4. Historico

> Por fim, criou-se a biblioteca histórico, responsável por criar um arquivo histórico à fim de armazenar os filmes assistidos pelos usuários, bem como acessar esse arquivo posteriormente para uso dessas informações, para impressão do histórico, ordenação, etc. 

##########################################################################

## Uso dos arquivos csv

### Arquivo usuarios.csv

> Cada linha do arquivo foi atribuida à um usuário, tendo cada linha o ID do usuário, seu nome, senha e seu código de atividade (1 para ativo e 0 para inativo), nessa respectiva ordem, como no exemplo a seguir:

```cpp
4,vinicius,am8H3z2pL,1
5,saulo,naosabeaminhasenha,0
6,jessica,uflixtop,1
```
### Arquivo historico.csv

> Nesse arquivo, cada linha foi atribuída à um filme assistido, com seu respectivo id de usuário, título do filme, data em que foi assistido e nota, como no exemplo à seguir. 
> PS.: Note que, o usuário 9 assistiu três filmes e, os três filmes, foram atribuídos à linhas diferentes. 

```cpp
8,Charlotte,12/12/1997,7.5
9,Love and Shukla,15/11/2012,5.5
9,Show Pieces,19/03/2001,5.6
9,Qian ren 3: Zai jian qian ren,12/04/2021,10.0
```