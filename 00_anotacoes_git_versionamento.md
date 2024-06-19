# CURSO DE GIT / VERSIONAMENTO

### COMANDOS.
* `gitignore` : Um arquivo para ignorar arquivos e pastas que voce nao quer enviar para repositorio remoto.
* `git --version`
* `'Q'` = Tecla que sai do Terminal Git.

### VERSIONAMENTO - 
* `VERSIONAMENTO` - Registra todas as mudanças de um projeto, que possibilita o 
    acesso de varias versoes anteriores do desenvolvimento de código. Colaborando
    com toda a equipe do projeto e depois fazendo a junção do projeto.

### GIT - SOFTWARE E FRAMEWORK.
* `GIT` - Sistema de versionmento de código e um conjuntos de software.
    Guarda Registros de versões de código, salva o momento do projeto em seu computador,
    e com algumas simples linhas de comando voce manda todo o seu projeto para um repositorio remoto.

### INSTALACAO GIT.
* `LINK DO GIT :`
    https://www.git-scm.com/downloads

### DOC GIT.
* `LINK DOC GIT :`
    https://www.git-scm.com/docs

### GITHUB DESKTOP
* `LINK GIT DESCKTOP :`
    https://desktop.github.com/

# GIT STATUS - TIPOS DE ESTADO DO GIT.

### `UNTRACKED`
* Um arquivo novo no projeto que ainda não foi adicionado ao controle de versão do Git.

### `UNMODIFIED`
* Um arquivo que já está mapeado pelo Git e não sofreu modificações desde o último commit.

### `MODIFIED`
* Um arquivo que já foi modificado desde o último commit.

### `STAGED`
* Um arquivo que foi adicionado à área de preparação (staging area) e está pronto para ser commitado.

## 1º CONFIGURANDO O GIT E REPOSITORIO LOCAL
* `git init :` :  Inicializa um repositório git vazio no diretório atual.

*  `git config --global user.name '<seu_nome_github>' `: Define o nome de usuário a ser associado aos commits no repositório globalmente.

* `git config --global user.email '<seu_email_github>'` : Define o email a ser associado aos commits no repositório globalmente.

* `git checkout -b <nome_branch>` : Cria uma nova branch com o nome especificado e muda para ela.

* `git remote add <usuario_github> <URL do seu repositorio online>` : Adiciona um repositório remoto com o nome especificado e a URL fornecida.

* `git remote -v` : Lista os repositórios remotos configurados, mostrando as URLs associadas a eles.

* `git remote rm <destination>` : A remoção do URL remoto do repositório apenas desvincula os repositórios locais e remotos. Isso não exclui o repositório remoto.

## 2º BUSCANDO UM REPOSITORIO ONLINE - CLONANDO
* `git clone <URL do seu repositorio online>` :
Este comando é utilizado para clonar um repositório online para o seu computador local. Ao executar este comando, o Git fará uma cópia exata do repositório remoto e o trará para o seu ambiente de trabalho local. A URL do seu repositório online deve ser substituída pela URL real do repositório que você deseja clonar.

## 3º COMANDOS PARA ENVIAR UM ARQUIVOS PARA SEU REPOSITORIO
* `git status` - Este comando mostra o estado atual do repositório, indicando quais arquivos foram modificados, adicionados ou removidos.

* `git add .` - Este comando adiciona todas as modificações feitas nos arquivos ao índice, preparando-os para serem commitados.

* `git status` - Após o comando `git add .`, este comando mostra novamente o estado atual do repositório, indicando as modificações que foram adicionadas ao índice.

* `git commit -m '<Descricao do Commit>'` - Este comando cria um novo commit com as modificações que foram adicionadas ao índice, e a mensagem entre aspas é a descrição do commit.

* `git push` - Este comando envia os commits locais para o repositório remoto.

* `git diff` - Este comando mostra as diferenças entre o estado atual do repositório e o último commit.

* `git log` - Este comando mostra o histórico de commits do repositório, exibindo informações como autor, data e mensagem de cada commit.

* `git restore` - Este comando desfaz as modificações feitas nos arquivos, restaurando-os para o estado do último commit.

* `git restore --staged <nome_do_arquivo>` - Este comando desfaz a adição dos arquivos ao índice, retirando-os da preparação para o commit.

* `git pull` - O comando "git pull" no Git é utilizado para atualizar o repositório local com as alterações realizadas no repositório remoto. Ele basicamente combina dois comandos: "git fetch" e "git merge".

## 4º VERIFICANDO ALTERACOES NO REPOSITORIO REMOTO ANTES DE TRAZER PARA REPOSITORIO LOCAL

* `git fetch` - O comando git fetch é usado para trazer as alterações do repositório remoto para o seu repositório local, sem mesclar (merge) essas alterações com o seu código local. Ele baixa os objetos e referências (como branches e tags) do repositório remoto especificado, mas não atualiza o seu branch local.

* `git diff <seu_usuario>/<sua_branch>` - O comando é usado para visualizar as diferenças entre o seu branch local e o branch remoto correspondente no repositório "origin".

## 5º GIT BRANCH

* `git log --oneline --decorate` : comando é usado no Git para fornecer uma visão compacta e informativa do histórico de commits. Este comando fornece uma lista concisa de commits, mostrando um commit por linha, junto com quaisquer referências (como ramificações ou tags) associadas a esses commits. Aqui está um resumo do que este comando faz:

* `git branch <nome_branch>` :  Comando que cria uma nova branch, mas nao entra na branch.

* `git checkout <nome_branch_criada>` : Comando que entra na branch criada.

* `git checkout -b <nome_branch>` : Comando que cria uma branch e ja entra na branch criada.