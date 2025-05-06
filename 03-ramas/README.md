# 3 🌿 Ramas, Merge y Conflictos en Git

<details>
  <summary><strong>🌱 Las ramas en Git</strong></summary>

### ¿Qué es una rama?
Una rama es una instantánea (snapshot) del estado del código.  
A nivel técnico, es un nuevo apuntador hacia una de las confirmaciones (commits).

### ¿Para qué sirven?
- Desarrollar de forma no lineal
- Fomentar el trabajo colaborativo
- Probar ideas sin afectar el código principal


    <img src="https://res.cloudinary.com/snyk/images/f_auto,q_auto/w_1240,h_384,c_scale/v1/wordpress-sync/image1-11/image1-11-1240x384.png" width="600" />
</details>
<details>
  <summary><strong> 🌱 Comandos basicos de Ramas </strong></summary>

  | Paso                            | Comando                                        | Descripción                                         |
|----------------------------------|------------------------------------------------|-----------------------------------------------------|
| 1. Crear una nueva rama          | `git branch mi-primera-rama`                   | Crea una nueva rama llamada `mi-primera-rama`.      |
| 2. Cambiar a la nueva rama      | `git switch mi-primera-rama`                   | Cambia a la rama `mi-primera-rama`.                 |

</details>
<details>
  <summary><strong>🔀 ¿Qué es fusionar ramas en Git?</strong></summary>

Las ramas en Git representan bifurcaciones del código para trabajar en paralelo.

Estas ramas pueden:

- ❌ Quedar en el olvido si no se integran.
- ✅ Ser fusionadas en otra rama como `main` o `develop`.

**Fusionar** significa incorporar los cambios realizados en una rama secundaria hacia otra rama principal, unificando los historiales y progresos.

</details>

<details>
  <summary><strong>🛠️ Cómo fusionar ramas paso a paso</strong></summary>

📌 Cambia a la rama donde quieres hacer la fusión (ejemplo: `main`):

   ```bash
   git checkout main
   ```
🔁 Fusión de la rama secundaria:

```bash
git merge nombre-de-la-rama
```
Ejemplo:

```bash
git merge my-branch
```

✅ Si no hay conflictos, se crea un nuevo commit automáticamente que une ambos historiales.

</details> <details> <summary><strong>📝 Opciones avanzadas del comando merge</strong></summary>
Puedes tener más control sobre el mensaje del commit de fusión con:

```bash
# Abre el editor para escribir el mensaje del merge
git merge --edit
```

```bash
# Evita que Git haga el commit automáticamente
git merge --no-commit
```
💡 Esto es útil cuando deseas revisar, modificar o agregar contenido antes de confirmar la fusión.

</details> <details> <summary><strong>🧩 Diagrama visual de una fusión</strong></summary>
A continuación se muestra un ejemplo visual de cómo funciona el merge en Git:

<img src="https://wac-cdn.atlassian.com/dam/jcr:c6db91c1-1343-4d45-8c93-bdba910b9506/02%20Branch-1%20kopiera.png?cdnVersion=2678" alt="Diagrama de fusión de ramas en Git" width="700"/>
</details>
<details>
  <summary><strong>🗑️ ¿Por qué y cómo eliminar ramas en Git?</strong></summary>


### 🧠 ¿Por qué eliminar ramas?

Cuando trabajamos con ramas (`feature/`, `fix/`, etc.), lo ideal es eliminarlas cuando:

- ✅ Ya se han fusionado con la rama principal (`main`, `develop`, etc.).
- 🧹 Queremos mantener limpio y ordenado nuestro repositorio.
- 🧭 Evitamos confusiones con ramas antiguas o sin uso.

Eliminar ramas es una buena práctica que forma parte del flujo profesional de trabajo con Git.

---

### 🛠️ Comandos para eliminar ramas

| Comando                                | Descripción                                                  |
|----------------------------------------|--------------------------------------------------------------|
| `git branch -d <nombre rama>`          | Elimina una rama local (solo si ya fue fusionada)            |
| `git branch -D <nombre rama>`          | Fuerza la eliminación de una rama local, aunque no se haya fusionado |
| `git push origin --delete <nombre rama>` | Elimina una rama remota (en GitHub, GitLab, etc.)          |

</details>

## Tipos de Uniones en Git

<details>
  <summary><strong>Fast-Forward (Avance Rápido)</strong></summary>
📌 Ocurre cuando la rama a fusionar está directamente adelante de la rama en la que estás. En este caso, Git avanza la referencia de la rama principal hacia el último commit de la rama de características.

  **Comando**:
  ```bash
  git merge <nombre-rama>
  ```
  
  <img src="../Imagenes/Fast.png" alt="Fast Forward" width="300"/>

</details> <details> <summary><strong>Unión Automática</strong></summary> 📌 Cuando no hay conflictos, Git fusionará las ramas automáticamente y no necesitarás hacer nada más.

  <img src="../Imagenes/Union.png" alt="Fast Forward" width="300"/>
</details> <details> <summary><strong>Unión Manual (Merge Commit)</strong></summary> 📌 Si existen conflictos entre las ramas, Git te pedirá que los resuelvas manualmente. Una vez que se resuelvan los conflictos, debes hacer un commit para completar la fusión.

Comando:
 ```bash
git merge <nombre-rama>
  ```

  <img src="../Imagenes/MergeManual.png" alt="Fast Forward" width="300"/>
</details>

## ¿Qué pasa cuando dos personas tocan el mismo código?
<details> <summary><strong>Conflictos de Merge</strong></summary> 📌 Si dos personas modifican la misma línea de código en diferentes ramas y luego intentan hacer un merge, Git detectará un conflicto. En ese caso, necesitarás resolverlo manualmente. Esto puede ocurrir cuando modificas líneas del mismo archivo en diferentes ramas y luego intentas fusionarlas. </details>

## Resolución de Conflictos
<details> <summary><strong>Resolución Manual</strong></summary> 📌Git te marcará el archivo con conflictos y podrás resolverlo editando el archivo directamente. </details> <details> <summary><strong>Herramientas de IDE</strong></summary> 📌 Muchos editores como VS Code, IntelliJ o GitHub Desktop tienen herramientas para ayudarte a resolver conflictos de manera visual. </details> <details> <summary><strong>Finalizar el Merge</strong></summary> 📌 Una vez resuelto el conflicto, debes hacer un `git commit` para completar el merge. </details> 

## 📋 Tabla de comandos de Git relacionados con commits

| 🛠️ Comando                                     | 🧠 ¿Qué hace?                                                                 |
|-----------------------------------------------|------------------------------------------------------------------------------|
| `git commit -m "mensaje"`                     | Crea un commit con un mensaje específico                                     |
| `git commit -am "mensaje"`                    | Añade cambios en archivos ya versionados (trackeados) y los commitea         |
| `git commit --amend -m "nuevo mensaje"`       | Reemplaza el último commit por uno nuevo con otro mensaje                    |
| `git reset --soft HEAD^`                      | Vuelve al commit anterior, manteniendo los cambios en staging                |
| `git reset --mixed HEAD^`                     | Vuelve al commit anterior, pero deja los cambios en el directorio de trabajo |
| `git reset --hard HEAD^`                      | Elimina los cambios y vuelve completamente al commit anterior (⚠️ peligroso) |
| `git reflog`                                  | Muestra todos los movimientos del puntero HEAD (útil para recuperar commits) |
| `git diff`                                    | Muestra diferencias entre los archivos modificados y el último commit        |
| `git diff --staged`                           | Muestra diferencias entre staging y el último commit                         |
| `git log`                                     | Muestra el historial completo de commits con mensajes y fechas               |
| `git log --oneline --graph`                   | Muestra el historial de commits en forma resumida y gráfica                  |
| `git show <hash>`                             | Muestra los detalles completos de un commit específico                       |
| `git cherry-pick <hash>`                      | Aplica un commit específico sobre tu rama actual                             |
