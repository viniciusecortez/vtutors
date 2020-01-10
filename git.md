---
layout: default
title: Git
---


# Git
## Sobre

Git é um sistema de controle de versões distribuído usado principalmente no desenvolvimento de aplicações. Porém, é possível utilizá-lo também para outras edições 


## Baixar

### Para Linux

No caso do linux, é possível que já tenha o git instalado. Para saber se existe uma versão do git, abra o terminal e escreva:
~~~bash
git -v
~~~

* Se for derivado de Debian
~~~bash
sudo apt-get update
sudo apt-get install -y build-essentials
sudo apt-get install -y git
~~~

* Se for derivado do Red Hat
~~~bash
sudo yum install git
~~~

* Se for derivado do archlinux
~~~bash
sudo pacman -Syu git
~~~

### Para windows
Como o git foi uma criação feita para linux é necessário instalar o bash disponibilizado pelo site oficial do git: [baixar](https://git-scm.com/download/win).

## Configurações iniciais
O git necessita de uma identificação para saber quem está fazendo as alterações. Ele faz isso da seguinte forma:
~~~bash
git config --global user.name "[Seu nome]"
git config --global user.email "[Seu email]" 
# Lembrando que é esse email que irá ser carimbado por serviços como o github ou gitlab
~~~



## Iniciando um repositório

Um repositório git é uma pasta a qual estará seu projeto, onde o git irá monitorar quais ações foram feitas. 
Para iniciá-lo é só colocar o seguinte comando no diretório que deseja:
~~~bash
git init
~~~ 


## Estrutura

A estrutura do git se baseia no seguinte sistema:
