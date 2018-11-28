# Práctica del curso de git, gitHub y Sourcetree
##Gabriel Lago Blasco

### ¿Qué comando utilizaste en el paso 11? ¿Por qué?
- *git reset --hard HEAD~1* 
- Uso reset --hard porque el enunciado pide perder los cambios realizados en el working copy

### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
- *reflog* 	
- Busco el hash del commit eliminado (061266c)
- *git reset --hard 061266c*

### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
- No causó conflicto porque se modificó git-nuestro en style. Style tiene todos los commits anteriores, git puede trazarlo sin que quepan dudas.
- Por eso devuelve 'Already up to date.', no hay cambios en paralelo que generen un conflicto.

### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
- Sí se generó un conflicto porque hubo modificaciones en paralelo sobre las mismas líneas en dos ramas

### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
- No causó conflicto, se añadieron las modificaciones sobre git-nuestro porque master absorvia la rama con los cambios. 

### ¿Qué comando o comandos utilizaste en el paso 25?
- *git log --graph --decorate --pretty-oneline*

### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
- No, porque se hicieron cambios en la rama title y se volvió a la rama master que estaba un commit por detrás. 
- No se podía hacer una lista con los commits.

### ¿Qué comando o comandos utilizaste en el paso 27?
- *git reset HEAD~1*

### ¿Qué comando o comandos utilizaste en el paso 28?
- *git commit - m "Descartados cambios tras merge title"*

### ¿Qué comando o comandos utilizaste en el paso 29?
- *git branch -D title* 
- (Había que forzar el delete porque title no estaba merged del todo)

### ¿Qué comando o comandos utilizaste en el paso 30?
- *git reset --hard ae1c441*

### ¿Qué comando o comandos usaste en el paso 32?
- *git checkout 3c4dfe8*

### ¿Qué comando o comandos usaste en el punto 33?
- *git checkout ae1c441*