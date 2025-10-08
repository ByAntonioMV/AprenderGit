# 🧠 Guía rápida de comandos Git

Este documento contiene los comandos esenciales para trabajar con **Git** desde la terminal o consola.  
Ideal para iniciar un nuevo proyecto o recordar los comandos más comunes.

---

## ⚙️ Configuración inicial
```bash
# Configura tu nombre de usuario global
git config --global user.name "TuNombre"

# Configura tu correo electrónico global
git config --global user.email "tuemail@example.com"

# Verifica la configuración actual
git config --list ``
```

## ⚙️ Crear y clonar repositorios
```bash
# Inicializa un nuevo repositorio en la carpeta actual
git init

# Clona un repositorio remoto
git clone https://github.com/usuario/repositorio.git
```

## ⚙️ Estados y seguimiento
```bash
# Muestra el estado actual de los archivos (nuevos, modificados, eliminados)
git status

# Agrega un archivo específico al área de preparación (staging)
git add nombre_archivo

# Agrega todos los archivos modificados
git add .

# Elimina un archivo del área de preparación
git reset nombre_archivo
```

## ⚙️ Commits
```bash
# Guarda los cambios en el historial con un mensaje descriptivo
git commit -m "tipo: descripción del cambio"

# Ejemplo
git commit -m "feat: agrega botón de descarga en el panel principal"

| Tipo         | Descripción                                                       | Ejemplo                                             |
| ------------ | ----------------------------------------------------------------- | --------------------------------------------------- |
| **feat**     | Se usa cuando agregas una **nueva funcionalidad**.                | `feat: añade sistema de autenticación JWT`          |
| **fix**      | Se usa para **corregir errores o bugs**.                          | `fix: corrige error en la validación de email`      |
| **docs**     | Para **cambios en la documentación** (README, comentarios, etc.). | `docs: actualiza guía de instalación`               |
| **style**    | Cambios de **formato o estilo**, sin afectar la lógica.           | `style: ajusta indentación en el archivo main.js`   |
| **refactor** | Cambios en el **código existente** sin cambiar su comportamiento. | `refactor: simplifica función de carga de archivos` |
| **test**     | Agrega o modifica **pruebas automatizadas**.                      | `test: añade test unitario para login`              |
| **chore**    | Tareas rutinarias del proyecto (dependencias, scripts, etc.).     | `chore: actualiza dependencias npm`                 |
| **perf**     | Optimiza el **rendimiento** del código.                           | `perf: mejora tiempo de carga de imágenes`          |
| **build**    | Cambios en el **sistema de compilación o dependencias externas**. | `build: configura webpack para producción`          |
| **ci**       | Cambios en la **integración continua o despliegue automático**.   | `ci: agrega pipeline de GitHub Actions`             |

# Ejemplo completo
# Añadir una nueva característica
git add .
git commit -m "feat: agrega vista de perfil de usuario"

# Corregir un bug
git add .
git commit -m "fix: resuelve error en la carga de archivos"

# Actualizar documentación
git add README.md
git commit -m "docs: agrega tabla de comandos Git"

```
