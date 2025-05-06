# 5. GitHub: Push, Pull y Pull Request

<details>
  <summary><strong>🔁 git push</strong></summary>

  **Función**: Envía los cambios desde tu repositorio local al repositorio remoto (por ejemplo, GitHub).

  **Usos comunes**:
  - `git push`: hace un envío básico.
  - `git push -u origin <rama>`: establece la rama remota como predeterminada para futuros `push`.
  - `git push -f`: fuerza el envío (⚠️ puede sobrescribir cambios de otros).
  - `git push -d origin <rama>`: elimina una rama en el repositorio remoto.
</details>
<details>
  <summary><strong>⬇️ git pull</strong></summary>

  **Función**: Descarga y fusiona los cambios desde el repositorio remoto al repositorio local.

  **Usos comunes**:
  - `git pull`: trae y fusiona la rama remota vinculada.
  - `git pull origin <rama>`: trae cambios de una rama específica del remoto.
  - `git pull --all`: trae cambios de todas las ramas remotas.

  💥 **Advertencia**: si tu versión local tiene cambios distintos, pueden generarse conflictos que tendrás que resolver manualmente.
</details>