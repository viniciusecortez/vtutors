---
layout: default
title: Git | Commit
nav_order: 3
parent: Git
---
 


* **Commit** - É um pacote de alterações que tem como metadados o nome, email e horário que foi feito. Além disso, as próprias alterações também tem a hora que foram feitas. O comando para empacotar as alterações é justamente:

~~~bash
git commit -m "Mensagem para identificar o que são as alterações"
~~~

Para mudar a mensagem do commit:
~~~bash
git commit -m "Nova mensagem" --amend
~~~

