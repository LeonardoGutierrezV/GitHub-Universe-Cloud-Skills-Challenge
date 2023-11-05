Para validar la versión instalada de Git

```bash
git --version
```
Para configurar Git, debe definir algunas variables globales: user.name y user.email. Ambas son necesarias para realizar confirmaciones.

Establezca su nombre en Cloud Shell con el siguiente comando. Reemplace <USER_NAME> por el nombre de usuario que quiere usar.

```bash
git config --global user.name "<USER_NAME>"
git config --global user.email "<USER_EMAIL>"
```
Ejecute el siguiente comando para comprobar que los cambios han funcionado:

```bash
git config --list
```

Dentro de la carpeta donde se pretende inicializar un repositorio Git debera ejecutar el siguiente comando.
Si está ejecutando la versión 2.28.0 o una posterior de Git, use el comando siguiente:

```bash
git init --initial-branch=main
```
O bien, use el siguiente comando:

```bash
git init -b main
```
En versiones anteriores de Git, use estos comandos:

```bash
git init
git checkout -b main
```
alternativamente puede utilizar:

```bash
gir init
git branch -M main
```

Después de ejecutar el comando de inicialización, debería ver una salida similar a la de este ejemplo:

```bash
Initialized empty Git repository in /home/<user>/Cats/.git/
```
Ahora, use un comando git status para mostrar el estado del árbol de trabajo

```bash
git status
```

Teniendo como resultado lo siguiente:

```bash
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
```

utilice el comando "ls -a" para visualizar el contenido de la carpeta que ahora es la estructura del arbol del repositorio de Git.

```bash
ls -a
```
