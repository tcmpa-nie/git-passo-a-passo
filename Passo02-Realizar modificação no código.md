# Passo 02 : Modificação no código

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



Uma vez que você vai estar utilizando o GITHUB para manter os arquivos de seu projeto, consideremos que o repositório foi criado adequadamente por meio dos formulários web disponíveis neste site.

![Figura : Criação de Repositório](<Passo01.a-Criacao do Repositório GITHUB.png>)


Após a criação do repositório, o fluxo de trabalho se inicia ao realizar a operação de _"clone"_ do repositório, que significa criar uma cópia do repositório em um diretório local de seu computador. Lembre que estamos considerando que você tem acesso a um terminal de comandos (cmd, bash, powershell,...) e que seu computador já tenha o [git](https://git-scm.com/) instalado.


Acesse o terminal de comando e digite:
```bash

$ git clone https://github.com/tcmpa-nie/git-passo-a-passo.git

```

onde _"https://github.com/tcmpa-nie/git-passo-a-passo.git"_ é a URL do seu repositório no GITHUB, como indicado abaixo 

![Figura : Criação de Repositório](<Passo01.b-URL repositório no GITHUB.png>)


Depois de executado o comando acima, você terá um diretório com o nome de seu repositório. O próximo passo é realizar uma modificação no código.
