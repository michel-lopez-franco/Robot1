# Comandos git

# 1. Sincronizar con el profesor

# Para traer cambios del upstream (profesor)

git fetch upstream

# Para fusionar cambios del upstream con tu rama actual

git merge upstream/main

# 2. Crear rama para cada tarea

git checkout -b tarea-1

# 3. Trabajar y hacer commits

git add .
git commit -m "Completada tarea 1"

# 4. Subir a MI fork

git push origin tarea-1

# 5. Crear Pull Request desde GitHub

# Verifica la configuración actual

git remote -v

Entendiendo "origin" y "upstream" en Git
Estos términos se refieren a remotos (repositorios remotos) en Git. Te explico cada uno:

Origin
Es el nombre por defecto que Git le da al repositorio del que clonaste tu copia local

Cuando haces git clone URL, Git automáticamente crea un remoto llamado "origin" apuntando a esa URL

Es tu punto de conexión principal con el repositorio remoto

Upstream
Es un término usado para referirse al repositorio original cuando has hecho un fork (bifurcación)

Te permite mantener tu fork sincronizado con el repositorio original

No es un nombre automático como "origin", lo defines manualmente

[Repositorio del profesor] (upstream)
↑
[Tu fork en GitHub] (origin)
↑
[Tu copia local]
