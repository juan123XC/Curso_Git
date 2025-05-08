# 🔄 8. Deshacer Cambios en Git
<details>
  <summary><strong>❓ ¿Cuándo deshacer cambios?</strong></summary>

Situaciones comunes donde necesitamos deshacer:

- 🛑 El proyecto dejó de funcionar después de un cambio.
- 🧠 Queremos recuperar código eliminado por error.
- 🗑️ Deseamos restaurar archivos eliminados.

Git nos ofrece herramientas tanto destructivas como no destructivas para estos casos.
</details>
<details>
  <summary><strong>⚠️ Comandos destructivos vs no destructivos</strong></summary>

- **Destructivos**: Modifican el historial de commits (¡úselos con cuidado!).
- **No destructivos**: Trabajan con el historial, pero **no lo modifican permanentemente**.

**Ejemplo**:
- `git reset` → destructivo
- `git revert`, `git checkout` → no destructivos
</details>

<details>
  <summary><strong>🔧 git reset</strong></summary>

Permite mover el puntero de HEAD y modificar el historial local.

- `--soft`: mantiene los cambios realizados en staging (index).
- `--hard`: **descarta completamente** los cambios, tanto del staging como del working directory.

```bash
git reset --soft HEAD~1
git reset --hard HEAD~1
git reset --soft <SHA>
git reset --hard <SHA>
⚠️ --hard borra cambios irreversiblemente si no están respaldados.
```
   <img src="https://miro.medium.com/v2/resize:fit:1400/1*lirDsZh5ZZP3l9EtulZEjw.png" width="400"/>
</details> 