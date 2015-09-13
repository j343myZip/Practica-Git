#**¿Que comando utilizaste en el paso 11? ¿Por que?**

		git reset --hard HEAD~1

	Por que reset lleva el puntero a la posición indicada (HEAD~1, posición actual -1) 	y restaura el working copy que había en ese momento.

#**¿Que comando o comandos utilizaste en el paso 12? ¿Por que?**

		git reflog 
		git reset --hard (identificador)
	
	Hay que mover el puntero al último commit, lo obtenemos de reflog

#**El merge del paso 13, ¿Causo algún conflicto? ¿Por que?**

		git merge master

	No causa ningún conflicto por que la rama htmly ha absorbido a master ya

#**El merge del paso 19, ¿Causó algún conflicto? ¿Por que?**

	Si,porqué se han hecho modificaciones sobre las mismas lineas en ambas ramas y en 	commits diferentes.
	
		git checkout htmlify
		git merge matrix 
	
#**El merge del paso 21, ¿Causó algún conflicto? ¿Por que?**
 
	No, por que absorbe todos los commits

#**¿Que comando o comandos utilizaste en el paso 25?**
 
		git log --graph

#**El merge del paso 26, ¿Podria ser fast forward? ¿Por qué?**
  
		git merge --no-ff title
	
	Si, podría por que ambas ramas están en una linea continua

#**¿Que comando o comandos utilizaste en el paso 27?**
 
		git reflog
		git reset (identificador)
	Obtenemos el identificador de antes del título

#**¿Que comando o comandos utilizaste en el paso 28?**

		git checkout -- poem.md 

#**¿Que comando o comandos utilizaste en el paso 29?**
  
		git branch -D title

#**¿Que comando o comandos utilizaste en el paso 30?**

		git reflog
		git reset --hard (Identificador)

	Obtenemos el identificador de antes del merge

#**¿Que comando o comandos usaste en el paso 32?**

		git reflog 
		git reset --hard (Identificador)

	Obtenemos el identificador del inicio

#**¿Que comando o comandos usaste en el punto 33?**

		git reflog 
		git reset --hard (Identificador)
	Obtenemos el identificador del estado final

