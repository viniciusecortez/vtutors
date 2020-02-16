---
layout: default
title: Git | Commit
nav_order: 4
parent: Git
---
 
# Commit 

* **Descrição** - É um pacote de alterações que tem como metadados o nome, email e horário que foi feito. Além disso, as próprias alterações também tem a hora que foram feitas, a mensagem e o hash, que é a identificação, do commit anterior. O comando para empacotar as alterações é justamente:

~~~bash
git commit -m "Mensagem para identificar o que são as alterações"
~~~

## Flag amend

A flag **amend** altera o último commit feito. Com ela é possível adicionar arquivos que tem alterações que foram esquecidas de serem colocadas nesse commit. 

Para mudar a mensagem do commit:
~~~bash
git commit -m "Nova mensagem" --amend
~~~

