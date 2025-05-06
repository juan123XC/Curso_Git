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

<details>
  <summary><strong>🔃 Pull Request (PR)</strong></summary>

  **Definición**: Es una solicitud para que los cambios realizados en una rama (por ejemplo, `feature`) sean revisados y fusionados en otra rama (como `main` o `develop`).

  **Cómo se hace**:
  1. Subes tu rama con `git push`.

     <img src="https://edteam-media.s3.amazonaws.com/community/original/a82fdc37-4541-4f99-bfd4-71e1f215c12e.png" width="400"/>

  2. En GitHub, vas a la pestaña **Pull Requests** y haces clic en **New Pull Request**.
  
     <img src="https://david-estevez.gitbooks.io/the-git-the-bad-and-the-ugly/content/assets/github-pr-04.png" width="400"/>

  3. Seleccionas las ramas origen y destino, y describes los cambios.
  
     <img src="https://truth.bahamut.com.tw/s01/202406/0ee9ab85b1ae1edd3dd718db0ca318ea.PNG" width="400"/>

  **Buenas prácticas**:
  - Enfocar la PR en una sola funcionalidad o mejora.
  - Explicar claramente los cambios usando texto, capturas de pantalla, GIF o video demostrativo.

  **Revisión de PR**:
  - Brindar comentarios claros y constructivos.
  - Evaluar si el cambio funciona correctamente y está bien integrado en el contexto del proyecto.
</details>