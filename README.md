
Nesse repósitorio vou alocar as documentações do GIT e GitHub, além de resumos e comandos mais utilizados com finalidade de reforçar meus estudos no versionamento de códigos.

## Documentação

[GIT](https://git-scm.com/docs/git/pt_BR)

[GitHub](https://docs.github.com/pt)


![Logo](https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png)


## Instalação

Instalação do GIT no linux

```bash

# add-apt-repository ppa:git-core/ppa
# apt update; 
# apt install git
```

### Configuração inicial

Verificar se o git foi instalado e sua respectiva versão;
```bash
 git --version
```
Configurar sua identidade no Git.
```bash
 git config --global user.name "Seu Nome"
 git config --global user.email "seu@email.com"
```
Definir branch padrão
```bash
 git config --global init.defaultBranch main
```
Complementares
```bash
 git config --global core.editor "idea"  # Define editor padrão.
 git config --global color.ui auto  # Habilita cores.
```
    
## Funcionalidades e Códigos utilizados

### Criando e clonando repositórios

- Adicionando um repositório local no GitHub

mkdir < nome do repostorio >

git init

git remote add origin URL-SSH

- Clonando um repositório remoto para local

mkdir < nome do repostorio >

git init

git clone URL-SSH <nome da pasta-opcional>

- Verificar informações sobre a conexão com o git.
```bash
git status 
```
### Gerenciando as alterações do repositório

```bash
 git add < nome_arquivo > # Adiciona o arquivo para a área de preparação.
 
 git add . # Adiciona todos os arquivos novos ou alterados para a área de preparação.
 
 git commit -m "Mensagem do Commit"
 
 git commit -am # Adiciona altereção de um arquivo existente + mensagem do commit.
 
 git push # "Empurra" os arquivos para o repositório remoto.

 git push -u origin main  # Envia e configura upstream.
```
Busca mudanças no repositório remoto
```bash
git fetch
```
- Busca e "Puxa" todas as alterações do repositório remoto para o local
```bash
git pull
```
### Trabalhando com Branches e tratando conflitos

Criando uma ramificação do projeto (Branch)
```bash
git checkout -b < nome_branch >
```
Mesclando uma ramificação com a branch principal
```bash
git merge < nome da branch alternativa > 
```
- Alguns comandos com branches
```bash
git branch # Lista todas as branches.
git branch -v # Lista todas as branches e seus respectivo commit.
git branch -d <nome_branch> # deleta uma branch.
```
- Conflitos

Algumas vezes podemos nos deparar com conflitos ao tentar dar um "push" para o servidor remoto, isso pode ocorrer, pois alguma outra alteração já foi feita e seu repositório local possivelmente está dessincronizado.

Primeiramente, se acalme e siga as instruções:

Dê um "Pull" no seu repositório local, para puxar todas as mudanças ocorridas no repositório remoto. Após isso verifique qual o(s) arquivo(s) conflitante. Acesse o arquivo e escolha qual a edição de fato constará neste; Salve e retorne para o console adicionando a modificação e comitando. Por fim dê o push.

## Guia Completo de Comandos

Acesse neste [link](https://web.dio.me/articles/git-cheat-sheet-guia-completo-de-comandos-968de4c10259?back=/home).

## Referência

 - [Digital Innovation One](Dio.me)
 - Versionamento de Código com Git e GitHub - Elidiana Andrade
 - Git Cheat Sheet - Guia Completo de Comandos - Otávio Guedes


