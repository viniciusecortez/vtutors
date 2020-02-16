---
layout: default
title: Git | Branches
nav_order: 4
parent: Git
---
 
# Git | Branches

## Branches

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

