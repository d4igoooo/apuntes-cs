## Inicialización y conexión con repositorio remoto

### 1. Preparar exclusiones (.gitignore)
Antes de hacer commit, crear el archivo `.gitignore` para no subir configuraciones del sistema o del editor:
```bash
# En Windows/Mac, excluir archivos del sistema y carpetas internas
.obsidian/workspace.json
.obsidian/workspace-mobile.json
.trash/
```

### 2. Inicializar y enlazar con GitHub
```bash
# 1. Posicionarse en la carpeta raíz
cd /ruta/a/tu/boveda

# 2. Iniciar el repositorio local
git init

# 3. Renombrar la rama principal a main (estándar actual)
git branch -M main

# 4. Agregar los cambios al área de preparación (staging)
git add .

# 5. Crear el primer commit
git commit -m "feat: commit inicial de la bóveda de apuntes"

# 6. Conectar con el repositorio remoto vacío creado en GitHub
git remote add origin [https://github.com/](https://github.com/)<tu-usuario>/<tu-repo>.git

# 7. Subir los cambios estableciendo la rama remota de seguimiento
git push -u origin main
```

### 3. Flujo diario de actualización
```bash
git add .
git commit -m "docs: actualizar apuntes de la semana"
git push
```