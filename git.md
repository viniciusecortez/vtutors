---
layout: default
title: Git
permalink: /git
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

Um sistema de controle de versão tem o objetivo de guardar as alterações que são feitas para ser possível voltar para um momento específico do código. Normalmente, esse grupo de alterações é agrupado. Esse grupo se chama, normalmente, de **commit**. 

Uma vez que você tenha salvo essas alterações nesse **commit**, será possível voltar nele para conseguir programar a partir dele ou saber a autoria dele.


## Definições

* **Config** - É o comando que irão ser colocadas as configurações

Para listá-las:
~~~bash
git config -l
~~~

Para configurar o nome e o email que irão aparecer nos commits:

~~~bash 
git config user.name "Seu nome"
~~~

~~~bash 
git config user.email "Seu email"
~~~

Por padrão essas confgurações são locais. Então é possível colocar a flag: --global para conseguir definir para todos os repositórios que você tem. Essa diferença foi feita com base de você ter mais de um email, por exemplo, se tiver um email corporativo.


* **Stage Area** - É a área de todos os arquivos que estão esperando para entrar o próximo commit. Eles ficam nessa área apartir do momento que você digita do comando:

~~~bash
git add <filename> # Para um arquivo específico
# ou
git add . # Para todos os arquivos 
~~~

* **Commit** - É um pacote de alterações que tem como metadados o nome, email e horário que foi feito. Além disso, as próprias alterações também tem a hora que foram feitas. O comando para empacotar as alterações é justamente:

~~~bash
git commit -m "Mensagem para identificar o que são as alterações"
~~~

Para mudar a mensagem do commit:
~~~bash
git commit -m "Nova mensagem" --amend
~~~



#### Branches

* **Branch** - É uma ramificação ou galho de uma árvore de commits. Se você está trabalhando sem o conhecimento de branches. Provavelmente, você está trabalhando na branch padrão do git, a **master**. Porém, é possível criar uma ramificação, que terá seus próprios commits que ficarão em paralelo com outros commits. E, o que é normalmente feito, integrada a master por meio de um **merge**.

Para criar um novo branch no commit atual:

~~~bash
git branch <nome branch> # Lembrando que o nome não deve conter espaços
~~~

* Para mudar para esse branch:

~~~bash
git checkout <nome branch>
~~~

* Para renomear seu branch

~~~bash
git branch <nome atual> -m <outro nome>
~~~

* Para deletar seu branch

~~~bash
git branch -D <nome> # Deve estar em outro branch para esse 'nome' ser deletado
~~~



* **Merge** - Isso irá mesclar um branch com o branch atual. Como se fosse unir ambos. Uma vez que foram unidos o branch que se uniu pode ser apagado sem ter a perda dos commits de estavam nele. O comando para fazer essa operação é:

~~~bash
git merge <outra branch>
~~~
