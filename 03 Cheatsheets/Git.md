## Inicializar repositorio (FORMA 1: git init)

> **Cuando usar**: Proyectos que ya existen localmente en el PC. Se utiliza cuando ya se empezó a escribir código en una carpeta en el computador y más adelante decides convertirla en un repositorio de Git para subirla a GitHub y respaldarla.
### 1. Preparar exclusiones (.gitignore)

Crear el archivo `.gitignore` en la carpeta a inicializar para no subir configuraciones del sistema o del editor (al hacer esto, NO marcar la creación del .gitignore ni README en Github):

```bash
# Obsidian
.obsidian/

# Para demás casos, usar gitignore.io

```

### 2. Inicializar y enlazar con GitHub

```bash
# 1. Ir a la carpeta a inicializar
cd /ruta/carpeta

# 2. Iniciar el repositorio local
git init

# 3. Renombrar la rama principal a main (estándar)
git branch -M main

# 4. Agregar los cambios al área de preparación (staging)
git add .

# 5. Crear el primer commit
git commit -m "feat: commit inicial de la bóveda de apuntes"

# 6. Conectar con el repositorio remoto vacío creado en GitHub
git remote add origin https://github.com/usuario/nombre-repositorio

# 7. Subir los cambios estableciendo la rama remota de seguimiento
git push -u origin main
```

### 3. Flujo de actualización

```bash
# Si es que no estamos en la carpeta del repositorio inicializado
cd /ruta/carpeta

git add .
git commit -m "descripción de los cambios"
git push
```

---
## Inicializar repositorio (FORMA 2: git clone)

> **Cuando usar**: Proyectos nuevos que parten desde cero o proyectos ya existentes en GitHub. Se utiliza cuando se configura el repositorio primero en la web (aprovechando el .gitignore o README de GitHub) o cuando se descargará el código de otra persona/equipo para empezar a trabajar en tu PC.
### 1. Crear repositorio en GitHub con exclusiones

En GitHub crear el repositorio seleccionando las casillas según el proyecto:
- Marcar **Add a README file**.
- Marcar **Add .gitignore** y elegir la plantilla del lenguaje (Java, C, etc.).

### 2. Clonar y enlazar automáticamente con la máquina local

```bash
# 1. Ir a la carpeta donde se quiere guardar el repositorio a clonar
cd /ruta/carpeta

# 2. Clonar el repositorio remoto (descarga la carpeta y configura git init + origin automáticamente)
git clone https://github.com/usuario/nombre-repositorio

# 3. Entrar a la carpeta recién creada por el clonado
cd nombre-repositorio
```

### 3. Flujo de actualización

```bash
# Si se abre una terminal nueva y no se está dentro del proyecto
cd /ruta/carpeta/nombre-repositorio

git add .
git commit -m "descripción de los cambios"
git push
```

---

