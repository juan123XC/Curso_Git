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
