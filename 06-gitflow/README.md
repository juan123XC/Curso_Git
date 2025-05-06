# 6 GitFlow: Ramas, Flujos y Consejos
<details>
  <summary><strong>🧭 ¿Qué es GitFlow?</strong></summary>

GitFlow es un flujo de trabajo colaborativo que define cómo usar Git de forma estructurada dentro de un equipo.  
Organiza el desarrollo en ramas con propósitos específicos, facilitando la gestión de versiones, pruebas y lanzamientos.

  <img src="https://files.programster.org/tutorials/git/flows/github-flow.png" width="400"/>
</details>

<details>
  <summary><strong>🌿 Ramas principales en GitFlow</strong></summary>

- **`main`**: Contiene el código en producción (estable).
- **`develop`**: Contiene el código en desarrollo y prueba.
- **`feature/*`**: Para nuevas funcionalidades. Se crean desde `develop` y regresan a `develop`.
- **`release/*`**: Para preparar nuevas versiones. Se integran a `main` y `develop`.
- **`hotfix/*`**: Para correcciones urgentes en producción. Se integran a `main` y `develop`.

  <img src="https://miro.medium.com/v2/resize:fit:1400/1*9yJY7fyscWFUVRqnx0BM6A.png" width="400"/>
</details>