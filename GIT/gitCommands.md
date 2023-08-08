# COMANDOS GIT

## Os 4 estados
* Não rastreado (untracked): O arquivo não faz parte do repositório. Ex: Novo arquivo;
* Adicionado (Added): O arquivo foi adicionado no versionamento do repositório;
* Modificado (modified): Significa que o arquivo esta diferente quando comparados com a última versão disponível no histórico;
* Não modificado (unmodified): O arquivo faz parte do repositório e está consolidado;
* Preparado (staged): Neste momento, o Git sabe que o arquivo foi modificado e agora está na área de preparação para ser consolidad;

## Ajuda

##### Geral
```
git help
```
##### Comando específico
```
git help add
```
```
git help commit
```
```
git help <qualquer_comando_git>
```
## Configuração

### Geral

##### Setar usuário
```
git config --global user.name "Seu Nome"
```
##### Setar email
```
git config --global user.email seuemail@seuemail.com.br
```
## Repositório Local

### Criar novo repositório
```
git init
```
### Verificar estado dos arquivos/diretórios
```
git status
```
##### Adicionar um arquivo em específico
```
git add meu_arquivo.js
```
##### Adicionar um diretório em específico
```
git add meu_diretorio
```
##### Adicionar todos os arquivos/diretórios
```
git add .
```
##### Comitar informando mensagem
```
git add commit -m "meu primeiro commit"
```
### Enviar arquivos/diretórios para o repositório remoto

O primeiro **push** de um repositório deve conter o nome do repositório remoto e o branch.
```
git push -u origin master
```
Os demais **pushes** não precisam dessa informação
```
git push
```

### Atualizar repositório local de acordo com o repositório remoto

##### Atualizar os arquivos no branch atual
```
git pull
```
##### Buscar as alterações, mas não aplica-las no branch atual
```
git fetch
```
### Clonar um repositório remoto já existente
```
git clone nome_repositorio.git
```
### Vincular repositório local com um repositório remoto
```
git remote add origin nome_repositorio.git
```