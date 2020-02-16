---
layout: default
title: Git | Config
nav_order: 2
parent: Git
---

# Git - Config

* **Descrição** - É o comando que irão ser colocadas as configurações

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

