# 4 GitHub

<details>
  <summary><strong> ¿Git y GitHub son lo mismo?</strong></summary>
  
  - **Git** es un sistema de control de versiones local.
  - **GitHub** es una plataforma en la nube para alojar repositorios Git y facilitar la colaboración.

    <img src="https://i.ytimg.com/vi/4K7NJPvsVDo/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLCIPFkBGsEWlPB-fogV5IVvCyGImw" width="400"/>
</details>

<details>
  <summary><strong> ¿GitHub es único?</strong></summary>

  No. Existen otras plataformas:
  - **Bitbucket**: Repositorios privados, integración con Jira (de Atlassian).
  - **GitLab**: Plataforma DevOps con integración de pruebas y despliegue (CI/CD).
</details>

<details>
  <summary><strong> Repositorios remotos</strong></summary>

  - Son repositorios alojados en un servidor (como GitHub).
  - Permiten sincronizar código entre distintos desarrolladores y dispositivos.

    <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEj7CpqGNI2ceZA6Kc5VJL6l2OopC2GE-4xCdduHCyo8ZhwUhxREhEfFkH0IthUE5HqVASxGXl2SET_CrKEMmmagqSxEeSfxxV9Hq_7wf41vHuXZhAOAeO59K0lvXY7MWSlV7VwLKINVf4k/s640/Repositorios.PNG" width="400"/>
</details>

<details>
  <summary><strong> Navegando por GitHub</strong></summary>

  Funcionalidades principales de un repositorio:
  - `Code`: Ver archivos del proyecto.
  - `Pull Requests`: Revisar y aceptar cambios.
  - `Actions`: Automatizar flujos de trabajo.
  - `Projects`: Organización de tareas.
  - `Wiki`: Documentación.
  - `Security`: Alertas de seguridad.
  - `Insights`: Estadísticas.
  - `Settings`: Configuración general.

    <img src="https://kinsta.com/wp-content/uploads/2023/02/save-repo-settings-1024x492.png" width="400"/>
</details>


<details>
  <summary><strong>📌 Generar y configurar clave SSH</strong></summary>

  ```bash
  # Ver llaves existentes
  ls -al ~/.ssh

  # Crear nueva clave SSH
  ssh-keygen -t rsa -b 4096 -C "tu.email@gmail.com"

  # Activar el agente SSH
  eval "$(ssh-agent -s)"

  # Añadir la clave
  ssh-add ~/.ssh/id_rsa

  # Copiar la clave pública (Windows)
  clip < ~/.ssh/id_rsa.pub
  ```
  🔗 Pegar en: [https://github.com/settings/ssh/new](https://github.com/settings/ssh/new)
</details>


<details>
  <summary><strong>📌 Conexión con repositorio remoto</strong></summary>

  ```bash
  # Agregar remoto
  git remote add origin <url>

  # Ver remotos
  git remote -v

  # Subir cambios
  git push origin <rama>

  # Obtener cambios
  git fetch

  # Eliminar ramas remotas obsoletas
  git remote prune origin
  ```
</details>

<details>
  <summary><strong>📌 Manejo de ramas</strong></summary>

  ```bash
  # Ver ramas locales y remotas
  git branch -a

  # Cambiar a una rama remota
  git switch <rama_remota>

  # Clonar un repositorio
  git clone <url>
  ```
  💡 Usa `origin` como nombre por defecto para el repositorio remoto principal.
</details>

