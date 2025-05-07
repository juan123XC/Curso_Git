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