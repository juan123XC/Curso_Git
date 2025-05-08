# 🧰 Hooks, Alias y Trucos de Git

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

</details>