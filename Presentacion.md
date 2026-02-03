# Presentación del Proyecto

**Autor:** _Miguel Angel Gutierrez_  
**Profesor:** _Javier Andres Gallego_

[![Git](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e0/Git-logo.svg/2560px-Git-logo.svg.png)]
## Descripción del repositorio
Este repositorio fue creado como parte de las **Tareas** del curso.  
El objetivo principal es demostrar el **flujo de trabajo básico** con Git y GitHub, incluyendo:

- Creación de un repositorio local
- Realización de commits
- Creación y edición de archivos
- Conexión con un repositorio remoto en GitHub
- Subida de cambios (push)
## Pasos realizados

### 1. Configuración inicial de Git (solo una vez)

```bash
# Configure mi nombre y correo. 

git config --global user.name "Tu Nombre Completo"
git config --global user.email "tucorreo@ejemplo.com"

# Cree una carpeta para el proyecto.

mkdir tarea
cd tarea

# Inicie el repositorio Git.
git init

# Verifique el estado.
git status```

### 2. Creación del primer archivo.

Lo cree en notepad++.
1. Abri notepad++ y cree un archivo nuevo vacio.
2. Lo guarde con el nombre de: "Presentacion".
3. Busque en el tipo de archivo "Markdown" con la extension ".md".
4. Ya seleccionado los parametros correctos, presione la tecla enter.

### 3. Primer commit.
```bash
# Agrege el archivo al área de preparación.
git add Presentacion.md

# Cree el commit con el mensaje del documento.
git commit -m "Creación inicial del archivo de presentación con la descripción del proyecto"

# Verifique el historial.
git log```
### 4. Creación del repositorio en GitHub.

1. Entre a https://github.com.
2. Hice todos los pasos para tener cuenta.
3. Cree un nuevo repositorio.
4. Lo configure como:
5. Nombre del repositorio: tareas.
6. Descripción: Repositorio para almacenar todas mis tareas.
7. NO aplique README, .gitignore ni licencia.

8. Clic en Create repository.
9. Copie la URL HTTPS.
10. Y la vincule a mi repositorio local.
```bash
# Vincule el repo local con el remoto
git remote add origin

# Verifique que se haya vinculado correctamente
git remote -v

# Subilos cambios
git push -u origin main```

### 5. Generar y Usar un Token de Acceso Personal (PAT)

1. En GitHub, Me meti a configuraciones.
2. Baje en el menú de la izquierda hasta Developer seƫngs. 
3. Seleccione Personal access tokens > Tokens (classic). 
4. Le di click en "Generate new token" como classic.
5. Le di el nombre de "token para tareas".
6. Expiracion: Elegi sin expiracion.
7. Scopes (Permisos) Marque la casilla repo.
8. Presione en "Generate token". 
9. Guarde mi token para luego introducirlo en el campo requerido.