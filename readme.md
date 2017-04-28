#Práctica Git, GitHub y SourceTree

**Fco. Javier Guerrero Carmona**

**¿Qué comando utilizaste en el paso 11? ¿Por qué?**
```git reset —hard HEAD~1``` Con el modificador *HEAD~1* deshago el último commit y con *--hard* vacío el **Working Copy**.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**
```git reflog``` para buscar el identificador del commit deshecho y posteriormente ```git reset --hard 20ba3fd```.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
No causo ningún conflicto, puesto que no se produce el **Merge**, ya que las dos ramas están apuntando al mismo **commit**, en el cual el archivo está igual. Me advierte con el mensaje **Already up-to-date**

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
Si, causó un conflicto, ya que en este caso la rama *Styled* apunta a un **commit** distinto del de la rama *Htmlify*, por tanto los archivos tienen cambios que generan el conflicto.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
No se produce conflicto, ya que al estar en línea las dos ramas *master* y *styled*, el merge es **fast-forward**, por lo que no se produce un nuevo commit. Entonces lo único que pasa es que la rama *master* y *styled* apuntan al mismo **commit**, por eso no se produce conflicto entre archivos, ya que ese commit sólo tiene una versión del mismo.

**¿Qué comando o comandos utilizaste en el paso 25?**
```git log --graph --decorate --pretty=oneline```

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
Si, podría ser perfectamente **fast-forward**, ya que no necesitábamos un nuevo commit, simplemente avanzar el puntero *master* a *title*.

**¿Qué comando o comandos utilizaste en el paso 27?**
```git reset HEAD~1```, para deshacer el **merge**. No pongo el modificador --hard para mantener los cambios en el **working copy**.

**¿Qué comando o comandos utilizaste en el paso 28?** 
```git checkout -- git-nuestro.md```

**¿Qué comando o comandos utilizaste en el paso 29?**
```git branch -D title```

**¿Qué comando o comandos utilizaste en el paso 30?**
```git reflog``` para localizar la referencia del **merge**, en este caso 02203e6 y después un ```git reset --hard 02203e6 ```

**¿Qué comando o comandos usaste en el paso 32?**
```git reflog``` para localizar la referencia del **commit inicial**, en este caso 692a220 y después un ```git reset --hard 692a220```

**¿Qué comando o comandos usaste en el punto 33?** 
```git reflog``` para localizar la referencia del **commit** donde poníamos el título, en este caso f435cea y después un ```git reset --hard f435cea```

