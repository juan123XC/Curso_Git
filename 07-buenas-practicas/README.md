# 7. Buenas Prácticas en Git

<details>
  <summary><strong>🎯 ¿Para qué sirven las buenas prácticas?</strong></summary>

- Mantienen un estándar común en el equipo.
- Facilitan la resolución de conflictos.
- Hacen que el historial de commits sea claro, legible y útil para auditorías o revisión.

    <img src="https://aelis.es/wp-content/uploads/2023/10/buenas-practicas-1.jpeg" width="400"/>
</details>
<details>
  <summary><strong>🕒 ¿Cada cuánto debería hacer un commit?</strong></summary>

- **Haz commits frecuentemente.**
- Es mejor **varios commits pequeños** que uno muy grande.
- Agrupa cambios lógicos relacionados (no mezcles múltiples funcionalidades en un solo commit).
- Frecuencia no significa desorden: **evita commits innecesarios** o sin sentido.
</details>
<details>
  <summary><strong>📝 Cómo escribir buenos mensajes de commit</strong></summary>

- Usa el **modo imperativo**: `Add`, `Fix`, `Update`, `Remove`.
- No uses punto final ni puntos suspensivos.
- Máximo **50 caracteres** en la línea principal.
- En el cuerpo, explica el “por qué” si es necesario.
- Añade contexto y usa buena puntuación.
</details>
</details>

<details>
  <summary><strong>🏷️ Prefijos comunes para commits (semántica)</strong></summary>

- `feat:` nueva funcionalidad.
- `fix:` corrección de error.
- `refactor:` reestructuración sin cambio en funcionalidad.
- `style:` cambios visuales o de formato (espacios, tabulaciones).
- `test:` agregando o actualizando pruebas.
- `docs:` documentación.
- `perf:` mejoras de rendimiento.
- `build:` configuración de build, despliegue.
- `ci:` cambios relacionados con integración continua.

</details>

<details>
  <summary><strong>🌿 Buenas prácticas al nombrar ramas</strong></summary>

- Sé **consistente** en la nomenclatura.
- Usa **verbos de acción** + funcionalidad o ticket.
- Incluye el ID del ticket o historia si usas herramientas como Jira.

</details>
