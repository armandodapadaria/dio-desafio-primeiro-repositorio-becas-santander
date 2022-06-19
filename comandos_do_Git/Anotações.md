# Lista de Comandos do Git :bookmark:



Para melhor entendimento, irei fazer algumas anotações dos comandos do Git

### Comandos Básicos

- **git config:** É utilizado para definir valores de configurações específicas do usuário como o e-mail, nome de usuário formato de arquivo, etc.

> ```
> git config --global user.email sam@google.com
> ```

- **git init:** Cria um novo repositório GIT.

> ```
> git init
> ```

- **git add:** É usado para adicionar arquivos presentes no diretório atual ao índice.

> ```
> git add temp.md
> ```

+ **git clone:** É utilizado para copiar o repositório do Github para a máquina atual.

> ```
> git clone alex@93.188.160.58:/path/to/repository
> ```

Porém, se uma cópia de trabalho de um repositório local for criada, deve-se utilizar:

> ```
> git clone /path/to/repository
> ```

- **git commit:** É utilizado para confirmar as alterações do arquivo .

> ```
> git commit –m “coloque sua mensagem aqui”
> ```

- **git status:** exibe a lista de arquivos alterados juntamente com os arquivos que ainda não foram adicionados ou confirmados.

> ```
> git status
> ```

- **git push:** Envia as alterações do arquivo para o Github.

> ```
> git push origin master
> ```

- **git checkout:** pode ser usado para criar ramos ou alternar entre eles.

> ```
> command git checkout -b <branch-name>
> ```

_Para apenas mudar de um ramo para o outro_

> ```
> git checkout <branch-name>
> ```

- **git remote:** Permite que o usuário se contecte a um repositório remoto.

> ```
> git remote –v
> ```

_E para se conectar a um servidor remoto:_

> ```
> git remote add origin <93.188.160.58>
> ```

- **git branch:** Pode ser usado para listar, criar ou excluir ramos.

> ```
> git branch
> ```

_Para excluir um ramo:_

> ```
> git branch –d <branch-name>
> ```

- **git pull:** Para mesclar todas as alterações presentes no repositório remoto para o diretório de trabalho local.

> ```
> git pull
> ```

- **git merge:** O comando **git merge** é usado para mesclar uma ramificação no ramo ativo.

> ```
> git merge <branch-name>
> ```

- **git diff:** É usado para listar os conflitos.

> ```
> git diff --base <file-name>
> ```

_Já o seguinte comando é usado para exibir os conflitos entre ramos about-to-be-merged antes de mesclá-los_

> ```
> git diff <source-branch> <target-branch>
> ```

_E para simplesmente listar os conflitos atuais_

> ```
> git diff
> ```

- **git tag:** A marcação é usada para marcar compromissos específicos com alças simples.

> ```
> git tag 1.1.0 <insert-commitID-here>
> ```

- **git log:** exibe uma lista de compromissos em uma ramificação, juntamente com os detalhes pertinentes.

> ```
> commit 15f4b6c44b3c8344caasdac9e4be13246e21sadw
> Author: Alex Hunter <alexh@gmail.com>
> Date:   Mon Oct 1 12:56:29 2016 -0600
> ```

- **git reset:** Serve para redefinir o índice e o diretório de trabalho para o estado do último commit.

> ```
> git reset --hard HEAD
> ```

- **git rm:**  Pode ser usado para remover arquivos do índice e do diretório de trabalho.

> ```
> git rm filename.txt
> ```

- **git stash:** ajuda a salvar as mudanças que não devem ser cometidos imediatamente, mas em uma base temporária.

> ```
> git stash
> ```

- **git show:** Para visualizar informações sobre qualquer objeto git.

> ```
> git show
> ```

- **git fetch:** permite que um usuário obtenha todos os objetos do repositório remoto que atualmente não residem no diretório de trabalho local.

> ```
> git fetch origin
> ```

- **git ls-tree:** Serve para exibir um objeto de árvore juntamente com o nome e o modo de cada item e o valor SHA-1 do blob.

> ```
> git ls-tree HEAD
> ```

- **git cat-file:** Usando o valor SHA-1, exiba o tipo de um objeto.

> ```
> git cat-file –p d670460b4b4aece5915caf5c68d12f560a9fe3e4
> ```

- **git grep:** permite que um usuário procure através das árvores de conteúdo frases e / ou palavras. Por exemplo, para pesquisar www.hostinger.com em todos os arquivos.

> ```
> git grep "www.hostinger.com"
> ```

- **gitk:** É a interface gráfica para um repositório local.

> ```
> gitk
> ```

- **git instaweb:** um servidor web pode ser executado em interface com o repositório local. Um navegador da Web também é automaticamente direcionado para ele.

> ```
> git instaweb –httpd=webrick
> ```

- **git gc:** Para otimizar o repositório através da coleta de lixo, que irá limpar arquivos desnecessários e otimizá-los.

> ```
> git gc
> ```

- **git archive:** permite que um usuário crie um arquivo zip ou tar contendo os componentes de uma única árvore de repositório.

> ```
> git archive --format=tar master
> ```

- **git prune:** s objetos que não têm ponteiros de entrada são excluídos.

> ```
> git prune
> ```

- **git fsck:** Para executar uma verificação de integridade do sistema de arquivos git. Todos os objetos corrompidos são identificados.

> ```
> git fsck
> ```

- **git rebase:** É usado para reaplicação de compromissos em outro ramo.

> ```
> git rebase master
> ```
