## MASTERUAH

### 1. Repositorio

```

$ git clone git@github.com:luciaayllon/masteruah.git
$ echo "# masteruah" >> README.md
$ git init
$ git commit -m "first commit"
$ git brach -M main
$ git push -u origin main

```

### 2. Commit inicial

```
$ git add .
$ git commit -m "commit inicial"
```



### 3. Push inicial

```
$ git push origin main
```

### 4. Añadir fichero 1.txt

```
$ touch 1.txt
$ git add .
$ git commit -m "añadido 1.txt"
```

### 5. Crear el tag v0.1 y subirlo

```
$ git tag v0.1
$ git push --tag origin main
```

### 6. Crear una rama y posicionarla

```
$ git branch v0.2
$ git checkout v0.2
```

### 7. Añadir fichero 1.txt

```
$ touch 2.txt
$ git add .
$ git commit -m "añadir 2.txt"

```

### 8. Crear una rama remota

```
$ git push origin v0.2
```

### 9. Merge directo

```
$ git checkout main
$ git merge v0.2 -m "merge v0.2"
```

### 10. Merge con conflicto

```
$ git checkout main
$ echo "lucia" >> 1.txt
$ git add .
$ git commit -m "lucia actu"

/////////////
$ git checkout v0.2
$ echo "Adios" >> 1.txt
$ git add .
$ git commit -m "adios actualizacion"

////////////

$ git checkout main
$ git merge v0.2
$ vim 1.txt
$ git add .
$ git commit -m "arreglo"
```

###  Listado de ramas 

```
$ git branch --merged
$ git branch --no-merged
```

### Arreglar el conflicto

```
$ vim 1.txt
$ git add .
$ git commit -m "arreglo "
```

### Borrar la rama

```
$ git tag v0.2
$ git branch -d v0.2
```

