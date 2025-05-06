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

<details>
  <summary><strong>✅ Ventajas de GitFlow</strong></summary>

- 🧩 Organización clara por tipo de rama.  
- 🔄 Permite múltiples versiones en paralelo.  
- 👥 Ideal para equipos grandes y colaborativos.  
- ⏳ Control preciso sobre pruebas y lanzamientos.
</details>

<details>
  <summary><strong>⚠️ Cuándo evitar GitFlow</strong></summary>

- 🚫 No es ideal para proyectos pequeños o personales.  
- 🐌 Sin CI/CD, puede ser lento y engorroso.  
- 📉 No favorece la entrega continua rápida.
</details>

<details>
  <summary><strong>💡 Consejos prácticos para GitFlow</strong></summary>

- 🧪 Automatiza pruebas en `develop` y `release` con GitHub Actions o Jenkins.  
- 📛 Nombra tus ramas claramente:  
  - `feature/login-auth`  
  - `release/v1.2`  
  - `hotfix/payment-bug`  
- 🧼 Elimina ramas después de fusionarlas.  
- 🔍 Usa Pull Requests para control de calidad.  
- 📅 No mezcles tareas no relacionadas en una misma release.
</details>

<details>
  <summary><strong>📊 Comparativa de Flujos</strong></summary>

| Flujo                | Ramas principales      | Ideal para...                        | Complejidad |
|----------------------|------------------------|--------------------------------------|-------------|
| **GitFlow**          | `main`, `develop`, etc.| Equipos grandes, apps complejas      | Alta        |
| **GitHub Flow**      | `main` + temporales    | Proyectos simples, despliegue rápido | Media       |
| **Trunk-Based Dev**  | `main` + efímeras      | CI/CD continuo, cambios mínimos      | Baja        |
| **Ship/Show/Ask**    | `main` + efímeras      | Equipos responsables y maduros       | Media       |
</details>

<details>
  <summary><strong>📌 Extras </strong></summary>

- Añade un diagrama visual del flujo GitFlow.  
- Muestra ejemplos reales de su implementación.  
- Finaliza con esta pregunta:  
  **¿Qué flujo se adapta mejor a tu equipo o proyecto actual?**
</details>