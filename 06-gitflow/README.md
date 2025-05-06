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

<details>
  <summary><strong>🔁 Flujos alternativos a GitFlow</strong></summary>

### 🔷 GitHub Flow
- Usa solo `main` y ramas temporales.
- Se trabaja con Pull Requests directamente hacia `main`.

    <img src="https://miro.medium.com/v2/resize:fit:1400/1*9yJY7fyscWFUVRqnx0BM6A.png" width="400"/>

### 🔷 Trunk-Based Development
- Solo `main` y ramas auxiliares de vida muy corta.
- Ideal con CI/CD continuo.

    <img src="https://statusneo.com/wp-content/uploads/2022/08/tbd_workflow.drawio-1-1.png" width="400"/>

### 🔷 Ship / Show / Ask
1. **Ship**: Fusionas directamente a `main`, sin revisión.  
2. **Show**: Fusionas con CI pero dejas registro visible.  
3. **Ask**: Usas una Pull Request para revisión antes de fusionar.  

    <img src="https://martinfowler.com/articles/ship-show-ask/ship-show-ask.png" width="400"/>

Este flujo requiere confianza, responsabilidad y automatización de pruebas.
</details>