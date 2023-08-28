
# Dio_Resumos_GIT/GITHub 
Repositório para armazenar resumos de GIT e GITHub do curso Versionamento de Código com Git e GitHub da [Dio](https://www.dio.me).

### 📚 Documentação
- [Documentação Git](https://git-scm.com/doc)
- [Documentação GitHub](https://docs.github.com/pt) 

### 💻 Resumos das Aulas
| Aulas | Resumos|
|-------|--------|
|Gravando alterações no repositorio local|[Rsumo]()|

## Configurações iniciais do Git
- Para configurar usuario (Assim todas as alteração feitas seram deste usuário) 
```
$ git config --global user.name "T-Justino" 
$ git config --global user.e-mail "t.justino.dev@gmail.com"
```
- Para consultar o nome da branch padrão
```
$ git config init.defaultBranch
```
- Para alterar  globlamente o nome da branch padrão para "main"
```
$ git config --global init.defaultBranch main
```
## Criação de repositório local
```
$ mkdir Nome_do_Repositorio
$ cd Nome_do_Repositorio
$ git init
```
## Enviando arquivos para repositorios
- Após ter adicionado e committado
```
$ git push -u origin Nome_da_branch
```
## Clonando repositório 

- Copiar a URL
- Abrir o Bash na pasta que deseja copiar o repositorio
- Digitar o seguinte comando
```
$ git clone URL
```
- Se quiser clonar com nome diferente
```
$ git clone URL Novo_nome
```
## Passando repositorio local para remoto
- Criar novo repositorio no GitHub
- Copiar a URL 
- Abrir GitBash na pasta local
- Digitar o seguinte comando 
```
    $ git remote add origin URL_copiada
```
- Verificando vinculo com repositório remóto
```
    $ git remote -v
```
## Trabalhando com branchs
- Criando nova branch
```
$ git checkout -b Nome_Da_Branch
```
- Acessando branch
```
$ git checkout Nome_Da_Branch
```
- Listar as branchs existentes no repositório (esteja na branch main)
```
$ git branch
```
- Listar ultimos commits das branchs (esteja na branch main)
```
$ git branch -v
```
- Mesclando branhs (esteja na branch que deseja mesclar e chame a outra branch com o comando)
```
$ git merge Nome_da_Branch
```
- Deletando branch (Precisamos antes mesclar as branchs)
```
$ git branch -d Nome_da_Brant
```
## Desfazendo alterações
- Caso tem dado *"git init"* na pasta errada e queira desfazer o versionamento dela
```
    $ rm -rf .git
```
- Restaurar arquivo
```
    $ git restore Nome_do_Arquivo.extensao
```
- Corrigir nome do commit 
```
    $ git commit --amend -m"Novo Commit"
```
- Desfazer commit voltando para o anterior
```
   // Opção Soft   Remove o commit mas adiciona os arquivos dos commits     
   posteriores na area de preparação:

   $ git reset --soft Colar_hash_do_commit_anterior 

   // Opção mixed  Remove o commit mas deixa os arquivos na area de trabalho 
   indicando que precisamos adicionar na area de preparação:

   $ git reset --mixed Colar_hash_do_commit_anterior

   // Opção hard  simplesmente apaga as alterações do ultimo commit:

   $ git reset --hard Colar_hash_do_commit_anterior 
```
- Histórico mais apronfundado sobre alterações dos commits
```
    $ git reflog 
```
- Remover arquivos da area de preparação
``````
    $ git reset Pasta/arquivo.extensao
``````
## Comandos recorrentes 
```
$ cat   // exibe arquivo de texto 
$ cd..    // volta uma pasta
$ touch   // cria arquivo vazio
$ git status // mostra status
$ git add nomedo_arquivo_para_adicionar_e_commitar
$ git add . // adiciona todas as pendencias para area de preparação 
$ git commit -m"mensagem de descrição da ação"
$ git log // mostra historico com horarios de alteações e autor da alteração 
// Ctrl + L (Limpa o console)
```
## Explicando comandos 
- O comando Git pull é uma junção dos comandos Git merce(mesclas as alterações) + git fetch (baixa as alterações)
## Observações
- Atalho para o editor do GitHub ( . ) dentro do repositório que deseja modificar