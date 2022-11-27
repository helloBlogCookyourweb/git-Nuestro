#Práctica GIT.
## Respuestas.

**- ¿Qué comando utilizaste en el paso 11? ¿Por qué? **
   
   `git reset --hard HEAD~1`  
    
    HEAD is now at 9f660e2 Added git-nuestro.md

 Con este comando, desahago los últimos cambios y en con el ~1 que se mueva al último commit, es decir que deje todo como estaba antes de ese último commit.
 Utilizando --hard  forzamos a eliminar esos cambios de nuestro repositorio local perdiendo los cambios en el working copy. 

**- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**  

    git reflog
    git reset --hard 9fdddba

   
   Con el primer comando, veo toda la informacion de los cambios realizados
   Con git reset --hard numero de commit al que quiero volver, forzando con --hard


**- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**  

No ha causado ningún conflicto, ya que estaba en orden. No ha habido cambios adicionales. La rama master entiendo que es la rama main, como se ha solicitado la subida. 
    

**- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Si, ya que hemos modificado el mismo fichero,  ha causado un conflicto. 
    
    
**-  El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

Si porque al cambiar de rama, ésta no tenía resuelto el conflicto con el fichero anterior.
   
    
**- ¿Qué comando o comandos utilizaste en el paso 25?**

   `git log --graph --decorate --pretty=oneline`, y me he instalado en el Xcode la extension git Graph
     
     


**- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Si porque no hay ninguna desviación de ramas en este punto.
    


**- Qué comando o comandos utilizaste en el paso 27?**

    
   ` git reset HEAD~1
    

**- ¿Qué comando o comandos utilizaste en el paso 28?**
  
`git checkout -- git-nuestro.md` 


**- ¿Qué comando o comandos utilizaste en el paso 29?**

`git branch -D title`
    

**- Qué comando o comandos utilizaste en el paso 30?**
 Primero un `git reflog`, con el que localizar la rama y luego un 
`git reset --hard 0d4fb64` 
    
**-¿Qué comando o comandos usaste en el paso 32?**

   
   `git reflog` 
   `git checkout 9f660e2` (primer commit)
 
**- ¿Qué comando o comandos usaste en el punto 33?**

>   `git reset --hard 5bbcd0f  
>   HEAD is now at 34b5362 Añadimos Titulo git-nuestro rama title



** Git tags
git tag inicial 9f660e2
 git tag styled 9f660e2 
git tag htmlify e83e291 
git tag title 5bbcd0f 

** Git final 
git checkout htmlify