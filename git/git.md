---
layout: default
title: Git
nav_order: 2
permalink: /git
has_children: true
---


# Git

## O que é Git?

**Git** é um sistema de controle de versão destribuído. Ele foi criado com o objetivo de substituir os sistemas de controle de versões existentes. Esses sistemas tinham a arquitetura de cliente-servidor. 

Essa arquitetura é baseada em que o cliente tem as versões finais dos arquivos e o servidor tem todas as alterações e às manda e recebe por meio de requisições de clientes. Porém, essa arquitetura pode causar muitos conflitos, uma vez que tenha mais de uma pessoa usando esse sistema. 

Esses conflitos acontecem quando há alteração no mesmo arquivo por mais de um usuário. Ou, num cenário pior, a alteração de vários arquivos por vários usuários. Isso causaria uma correção de conflitos infinita.

Porém, o git não se utiliza desse sistema. Ele é um sistema que tem a característica de ser distribuído. O que quer dizer que cada usuário que tem um repositório git obtem, automáticamente, todas as alterações que já foram feitas nesse repositório.

### Como funciona o git?

Uma coisa dúvida que pode ocorrer é como ele consegue agrupar todas essas alterações sem que a pasta fique pesando GB de espaço. E isso acontece por ter um sistema que uni (**tar**), compacta (**gzip**) e encripta (**sha1**) os arquivos. Além disso, as alterações funcionam com o sistema de patch que é basicamente um arquivo de diferença entre o estado anterior e atual dos arquivos. Ou seja, ele só armazena as diferenças.

Ele coloca todas essas modificações dentro de uma pasta que transforma a pasta que ela está em um repositório git. Essa pasta é **.git** . 

## O que é um sistema de controle de versão

Um sistema de controle de versão tem o objetivo de guardar as alterações que são feitas para ser possível voltar para um momento específico do código. Normalmente, esse grupo de alterações é agrupado. Esse grupo se chama **commit**. 

Uma vez que você tenha salvo essas alterações nesse **commit**, será possível voltar nele para conseguir programar a partir dele ou saber a autoria dele.


## Fluxo básico do git

* Primeiramente, é necessário  [baixar o git]({{site.baseurl}}git/baixar.html).

* Após ter baixado, para criar um repositório, é necessário iniciar o repositório dentro da pasta do  seu projeto.

~~~bash
git init
~~~

* Após isso deverá configurar para colocar suas credenciais do git. [Mais informações>>]({{site.baseurl}}git/config)


~~~bash
git config --global user.name "Seu nome"

git config --global user.email "Seu email"
~~~

* Depois você adiciona seus arquivos a stage área. [Mais informações>>]({{site.baseurl}}git/add)

~~~bash
git add .
~~~

* Depois você fará seu primeiro commit. [Mais informações>>]({{site.baseurl}}git/commit)

~~~bash
git commit -m "Mensagem referente as alterações"
~~~
