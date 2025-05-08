# 🧰9 Hooks, Alias y Trucos de Git

<details>
  <summary><strong>🔗 ¿Qué es un Hook?</strong></summary>

Un **hook** (gancho) es un script que se ejecuta automáticamente cuando ocurre un evento en Git.  
Tipos:

- **Del lado del cliente**: afectan solo el repositorio local.
- **Del lado del servidor**: se ejecutan en GitHub, GitLab u otros para validar cambios entrantes.

📁 Se ubican en `.git/hooks/`


<img src="https://miro.medium.com/v2/resize:fit:900/0*XACPPB4jjM7dqUu4.png" width="400"/>

</details>

<details>
  <summary><strong>💻 Hooks del lado del cliente</strong></summary>

- `pre-commit`: ejecuta verificaciones previas al commit (ideal para linters o restricciones).
- `prepare-commit-msg`: modifica o agrega contenido al mensaje del commit.
- `commit-msg`: valida que el mensaje del commit cumpla reglas.
- `post-commit`: útil para notificar eventos (por ejemplo, vía Slack).
- `pre-push`: ejecuta pruebas antes de hacer push.
- `post-checkout` y `post-merge`: acciones como limpieza de archivos o ramas al cambiar de contexto.

✅ Solo necesitas crear scripts con permisos de ejecución en `.git/hooks/`.
</details>

<details>
  <summary><strong>🌐 Hooks del lado del servidor</strong></summary>

Usados en plataformas como GitHub o GitLab para automatizar validaciones:

- `pre-receive`: verifica si los commits cumplen requisitos y si el usuario tiene permisos.
- `update`: controla qué actualizaciones se permiten.
- `post-receive`: puede enviar correos, actualizar interfaces o sincronizar ramas.

<img src="https://d8it4huxumps7.cloudfront.net/uploads/images/652f71f725c60_git_hooks_01.jpg?d=2000x2000" width="400"/>

💡 Muy útiles para controlar calidad, seguridad o automatización de despliegues.
</details>

<details>
  <summary><strong>🛠️ Cómo crear tu propio Hook</strong></summary>

Pasos básicos:

1. Ve a `.git/hooks/`
2. Crea un archivo con el nombre del hook (por ejemplo: `pre-commit`)
3. Escribe el script que deseas ejecutar (puedes usar Bash, Python, etc.)
4. Asegúrate de que tenga permisos de ejecución con `chmod +x`.

Ejemplo: evitar commits vacíos

```bash
#!/bin/bash
if git diff --cached --quiet; then
  echo "No hay cambios para guardar"
  exit 1
fi
```

</details>

<details>
 <summary><strong>⚡ Alias personalizados en Git</strong></summary>
Un alias te permite definir un comando corto para usar en vez de uno largo.

Ejemplo de configuración:

``` bash
git config --global alias.co checkout
git config --global alias.st status
```
Ahora puedes escribir:
```bash
git co main
git st
```
¡Mucho más rápido!

</details>

<details>
 <summary><strong># 🧠 Trucos avanzados en Git</strong></summary>

##  Gestión temporal de cambios

| Comando                                | Descripción                                                                 |
|----------------------------------------|-----------------------------------------------------------------------------|
| `git stash`                            | Guarda los cambios actuales sin confirmarlos.                              |
| `git stash -u`                         | También guarda archivos no rastreados.                                     |
| `git stash pop`                        | Recupera y aplica los últimos cambios guardados con `stash`.               |

---

##  Trabajar con commits específicos

| Comando                                | Descripción                                                                 |
|----------------------------------------|-----------------------------------------------------------------------------|
| `git cherry-pick <SHA>`               | Aplica un commit específico de otra rama a la actual.                      |
| `git commit --amend -m "mensaje"`     | Modifica el último commit (mensaje o contenido).                           |
| `git revert <SHA>`                    | Revierte los cambios de un commit creando un nuevo commit inverso.         |

---

##  Diagnóstico de errores

| Comando                                | Descripción                                                                 |
|----------------------------------------|-----------------------------------------------------------------------------|
| `git bisect`                           | Inicia una búsqueda binaria para encontrar el commit que causó un bug.     |
| `git bisect start`                     | Comienza el proceso de búsqueda.                                           |
| `git bisect bad`                       | Marca el estado actual como defectuoso.                                    |
| `git bisect good`                      | Marca un estado anterior como funcional.                                   |
| `git bisect reset`                    | Finaliza el proceso de búsqueda.                                           |

---

##  Recuperación de archivos y ramas

| Comando                                | Descripción                                                                 |
|----------------------------------------|-----------------------------------------------------------------------------|
| `git checkout <SHA> -- archivo.txt`   | Restaura un archivo desde un commit anterior.                              |
| `git restore --source=<SHA> archivo`  | (Git moderno) Alternativa a `checkout` para restaurar archivos.            |
| `git reflog`                           | Muestra el historial de movimientos de HEAD, incluso los descartados.      |
| `git reset --hard <SHA>`              | Restaura el repositorio completamente a un estado anterior (⚠️ destructivo).|

---

##  Trucos y utilidades adicionales

| Comando                                | Descripción                                                                 |
|----------------------------------------|-----------------------------------------------------------------------------|
| `git config --global alias.st status` | Crea un alias para abreviar comandos (en este caso, `git st`).             |
| `git shortlog -sn`                    | Muestra una tabla de contribuciones por autor.                             |
| `git diff --staged`                   | Muestra diferencias de archivos que están en staging.                      |
| `git log --oneline --graph --all`    | Visualiza el historial como un árbol compacto.                             |
| `git blame archivo.txt`              | Muestra línea por línea quién hizo cada cambio.                            |
| `git clean -fd`                       | Elimina archivos no rastreados y carpetas (⚠️ irreversible).               |
| `git show <SHA>`                     | Muestra los detalles de un commit específico.                              |

---

##  Recomendaciones para usar estos comandos

- 🔒 Haz respaldos antes de usar comandos destructivos como `reset --hard` o `clean`.
- 🧪 Usa `stash` para no perder cambios en pruebas rápidas.
- 🕵️‍♀️ Usa `bisect` cuando un bug aparece misteriosamente después de varios commits.
- 👨‍💻 Configura **alias** para los comandos que más repites.
</details>




<img src="https://external-preview.redd.it/hgFzqyyYzVEnzpImswHxWKjdpn5l4aBQbOIgfnGiBD4.jpg?width=640&crop=smart&auto=webp&s=9f82a68f3668daf1f77fdef40e8d3e8e3f04bdd6" width="400"/>
