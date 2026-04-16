# Passo 02 : Ciclo de Modificação de artefatos

Tendo _clonado_ o repositório para o seu computador, você deve habilitar esta cópia para receber as modificações necessárias ( adicionar, remover ou alterar arquivos e diretórios). Isto é feito criando-se um **_branch_** (ou ramificação) baseada na versão corrente do código do repositório ( geralmente denominada **_main_**). O git cria o registro de como estavam os arquivos (nomes, diretórios e seus conteúdos), permitindo assim identificar _**TODAS**_ as alterações feitas a partir deste momento.

Você não deve realizar nenhuma alteração sem antes criar um _**branch**_.

## Criando um novo _branch_

![Criar um novo Branch](<Passo02.a-Criar Branch.svg>)

Sua próxima tarefa será criar um novo _**branch**_, então acesse agora o terminal de comandos e digite:
```bash

$ git checkout -b [nome-do-branch] 

```

O _**[nome-do-branch]**_ deve ser ÚNICO, portanto é uma boa idéia adicionar nele seu nome, data ou código de O.S. e/ou tarefa.

A partir deste momento você pode iniciar as alterações que julgar necessárias na cópia do repositório.


Vale lembrar que as alteraçoes se aplicarão **SOMENTE** à sua cópia local do repositório, e desta forma não interferirão no trabalho dos outros membros da equipe, nem serão vistas (por enquanto) no GITHUB.


## Área de Staging do _**git**_

O _git_ é um sistema de controle de versão de arquivos _distribuído_, o que significa que após realizar a _clonagem_ do repositório remoto, o usuário trabalha totalmente _offline_, dependendo somente dos recursos de seu computador para realizar as alterações.

Para gerenciar as alterações nos arquivos, o _git_ se utiliza de uma estratégia simples e poderosa: ele mantém os arquivos em áreas distintas durante seu ciclo de alterações, que são:
 - **Diretório de Trabalho** (Working Tree): Onde você edita seus arquivos. Os arquivos recém adicionados ao projetos ficam registrados nesta área, **_sem_** que o _git_ guarde cada alterações sofridas por eles.

 - **Staging Area** (Índice): O _git_ passa a gerenciar os arquivos registrados nesta área (staging). É necessário que você indique o momento mais adequado para que os arquivos passem ao controle de alterações do _git_. Para isso, deve-se usar o seguinte comando.
 ```bash
   $ git add .
 ```
 
 - **Repositório Local Git** (Commit): Após realizar uma ou mais alterações nos arquivos da _staging area_, você aplica o comando _commit_ de forma a estabelecer uma espécie de marca d'agua nos arquivos do repositório, indicando uma posição no histórico do repositório que poderá ser replicada para os outros membros da equipe. Para isso, deve-se usar o seguinte comando.
 ```bash
   $ git commit -m "Mensagem que será associada a este commit"
 ```


Vale lembrar que este ciclo ocorre somente no seu computador, com o git registrando todos os marcos de alteração (commits) em seu _**repositório local**_.


## Enviando as alterações para o repositório remoto

Após ter realizado uma ou mais vezes o ciclo de alterações descrito anteriormente e estar satisfeito com o resultado de suas alterações, você pode enviá-las para o repositório remoto de origem no GITHUB, de forma a permitir que suas modificações sejam posteriormente aplicadas à _branch_ principal do código fonte. Lembre-se que você deve estar trabalhando na sua  _branch_ e caso não lembre o nome, use :

```bash
$ git status
```

Tudo pronto, então basta só executar o comando :

```bash
$ git push -u origin [nome-do-seu-branch] 
```

A partir deste momento o git envia seus arquivos alterados para o repositório remoto no GITHUB, organizados sob a identificação de seu _branch_, como ilustrado abaixo.

![alt text](Passo02-GitPull-ViewBranch.png)


O próximo passo é criar um _"**pull request**"_

![alt text](Passo02-GitPullRequest01.png)
