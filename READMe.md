
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
