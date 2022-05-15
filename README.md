
# Primeiro entregável da sprint 2 

## Descrição da atividade

Nesta atividade deverá ser criado o arquivo Readme com a descrição dos comando utilizados nas aulas de git e github.

## Comando de configuração

```
git config --global user.name "nome" -> Configura o nome do usuário
git config --global user.email "email" -> Configura o e-mail do usuário
```

## Comando de inicialização e clonagem

```
git init -> Inicia um repositório vazio
git clone "url do repositorio" -> Clona um repositório já existente
```

## Demais comandos 

### Setar ferramenta de merge
```
git config --global merge.tool vimdiff -> Setar ferramenta de merge
git config --global core.excludesfile ~/.gitignore -> Setar arquivos a serem ignorados
git config --list -> Listar configurações
git status -> Verificar estado dos arquivos/diretórios
```

### Adicionar arquivo/diretório (staged area)

```
git add meu_arquivo.txt -> Adicionar um arquivo em específico
git add meu_diretorio -> Adicionar um diretório em específico
git add . -> Adicionar todos os arquivos/diretórios
git add -f arquivo_no_gitignore.txt -> Adicionar um arquivo que esta listado no .gitignore (geral ou do repositório)
```
	
### Comitar arquivo/diretório

```
git commit meu_arquivo.txt -> Comitar um arquivo
git commit meu_arquivo.txt meu_outro_arquivo.txt -> Comitar vários arquivos
git commit meuarquivo.txt -m "minha mensagem de commit" -> Comitar informando mensagem
```

### Remover arquivo/diretório

```
git rm meu_arquivo.txt -> Remover arquivo
git rm -r diretorio -> Remover diretório
```

### Visualizar histórico

```
git log -> Exibir histórico
```

### Desfazendo operações

```
git checkout -- meu_arquivo.txt -> Desfazendo alteração local (working directory)
```

### Repositório Remoto

```
git remote -> Exibir os repositórios remotos
git remote -v -> Exibir os repositórios remotos
git remote add origin git@github.com:leocomelli/curso-git.git -> Vincular repositório local com um repositório remoto
git remote show origin -> Exibir informações dos repositórios remotos
git remote rename origin curso-git -> Renomear um repositório remoto 
git remote rm curso-git -> Desvincular um repositório remoto
git push -> Enviar arquivos/diretórios para o repositório remoto
```

### Atualizar repositório local de acordo com o repositório remoto

```
git pull -> Atualizar os arquivos no branch atual
git fetch -> Buscar as alterações, mas não aplica-las no branch atual
git clone git@github.com:leocomelli/curso-git.git -> Clonar um repositório remoto já existente
```
	
### Branches

```
git branch bug-123 -> Criando um novo branch
git checkout bug-123 -> Trocando para um branch existente
git checkout master -> Voltar para o branch principal (master)
git branch -d bug-123 -> Apagando um branch
git branch -> Listar branches
git branch -v -> Listar branches com informações dos últimos commits
git branch --merged -> Listar branches que já foram fundidos (merged) com o **master**
git branch --no-merged -> Listar branches que não foram fundidos (merged) com o **master**
```

###Stash

```
git stash -> Criar um stash
git stash list -> Listar stashes
git stash apply -> Voltar para o último stash
git stash apply stash@{"indíce do stash desejado"} -> Voltar para um stash específico
git stash branch meu_branch -> Criar um branch a partir de um stash
```

## Autor

- [@carloseducorreia](https://www.github.com/carloseducorreia)

## Referencia
- https://gist.github.com/leocomelli/2545add34e4fec21ec16
