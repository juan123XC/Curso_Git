# 2 Inicia tu Proyecto con Git & GitHub 🧑‍💻
### Aprenderas conceptos como **Estados y Commmits**📝
<details>
  <summary><strong> 📌 Paso 1: Crear tu Proyecto con Git </strong></summary>
  
<div style="display: flex; justify-content: space-between; align-items: flex-start;">

<div style="flex: 2; padding-right: 20px;">


1. Abre tu terminal y crea una carpeta para tu proyecto:
   ```bash
   mkdir mi-proyecto
   cd mi-proyecto
   ```

2. Inicializa Git en esa carpeta:
   ```bash
   git init
   ```
   Esto crea un repositorio Git vacío en tu carpeta.

3. Crea un archivo inicial:
   ```bash
   echo "# Mi primer proyecto con Git" > README.md
   ```
</div> <img src="https://i.ytimg.com/vi/sk5UCZxNjBk/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLDsHlw0dqysDHz-kQ2xnPu3eMYqgA" alt="git init" width="280" style="align-self: center; border-radius: 10px;" /> </div> </details> 
</details>

<details>
  <summary><strong> 🔍 Paso 2: Verifica el Estado de los Archivos </strong></summary>
  <div style="display: flex; justify-content: space-between; align-items: flex-start;">

<div style="flex: 2; padding-right: 20px;">

  
Usa este comando para ver en qué estado están tus archivos:
```bash
git status
```

Los archivos pueden estar en uno de tres estados:

| Estado       | Significado                                                                 |
|--------------|------------------------------------------------------------------------------|
| 📝 Modified  | El archivo fue modificado pero aún no está listo para confirmar (commit).    |
| 📥 Staged    | El archivo fue agregado al área de preparación (*stage*) para confirmar.    |
| ✅ Committed | El archivo ya fue registrado en el historial del repositorio.               |
| 🚫 Untracked | El archivo no está siendo rastreado por Git, es decir, no ha sido agregado al área de *staging* ni al repositorio. |


</div> <img src="https://nulab.com/static/d13cdc1344230f603d17b31a5cbd1dae/5a190/02.png" alt="git init" width="500" style="align-self: center; border-radius: 100px;" /> </div> </details> 
</details>