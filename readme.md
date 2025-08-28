
```
📁 Estructura recomendada:
text
repo-del-profesor/
├── README.md
├── material-clases/
├── ejercicios/
└── estudiantes/
    ├── michel-lopez-franco/
    │   ├── tarea-1.md
    │   ├── tarea-2.py
    │   └── proyecto-final/
    ├── estudiante-2/
    └── estudiante-3/
```
🔄 Flujo de trabajo paso a paso:
1. Configuración inicial del profesor:
bash
# Crear rama estudiantes
git checkout -b estudiantes

# Crear estructura de carpetas
mkdir -p estudiantes/michel-lopez-franco
mkdir -p estudiantes/estudiante-2
# etc...

git add .
git commit -m "📁 Crear estructura para estudiantes"
git push origin estudiantes
2. Tu flujo como estudiante:
bash
# Sincronizar con el repositorio
git fetch upstream
git checkout estudiantes
git pull upstream estudiantes

# Crear tu rama personal
git checkout -b michel-tarea-3

# Trabajar en tu carpeta personal
cd estudiantes/michel-lopez-franco
# Crear archivos de tarea...

# Commit y push
git add .
git commit -m "✅ Tarea 3 completada - Michel Lopez"
git push origin michel-tarea-3
