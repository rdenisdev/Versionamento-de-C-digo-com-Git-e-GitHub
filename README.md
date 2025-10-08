
## Documentação

[GIT](https://git-scm.com/docs/git/pt_BR)

[GitHub](https://docs.github.com/pt)


![Logo](https://git-scm.com/images/logos/downloads/Git-Logo-2Color.png)


## Instalação

Instalação do GIT no linux

```bash

# add-apt-repository ppa:git-core/ppa
# apt update; apt install git
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
  git config --global core.editor "idea"  # Define editor padrão
  git config --global color.ui auto  # Habilita cores
```
    
## Funcionalidades e Códigos utilizados

### Criando e clonando repositórios

- Adicionando um repositório local no GitHub
mkdir <nome do repostorio>

git init

git remote add origin URL-SSH

- Clonando um repositório remoto para local

mkdir <nome do repostorio>

git init

git clone URL-SSH <nome da pasta-opcional>

- git status -> Verificar informações sobre a conexão com o git.


## Referência

 - [Digital Innovation One](Dio.me)
 - Versionamento de Código com Git e GitHub - Elidiana Andrade


