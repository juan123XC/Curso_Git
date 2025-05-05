
# 1. Introducción a Git


<details>
  <summary><strong>🧠 ¿Qué es un Control de Versiones?</strong></summary>

<p align="justify">
  <img align="right" src="https://dinahosting.com/blog/upload/2018/06/Control-de-versiones.jpg" width="220" style="margin-left: 15px; border-radius: 10px;" />

  Un <strong>control de versiones</strong> es un sistema que registra cada cambio realizado en los archivos de un proyecto. Permite:
</p>

- 📜 <strong>Llevar un historial completo de cambios.</strong>  
- 🧍 <strong>Saber</strong> *quién* hizo el cambio y *cuándo*.  
- 🔐 <strong>Mantener la seguridad y consistencia del código.</strong>  
- 🔄 <strong>Ofrece flexibilidad: no obliga a un desarrollo lineal.</strong>


</details>


<details>
  <summary><strong>📜 Breve Historia</strong></summary>

| Año   | Evento                                                    |
|-------|-----------------------------------------------------------|
| 1990  | Nace **CVS**, el primer sistema de control de versiones. |
| 2005  | Se crea **Git**, impulsado por **Linus Torvalds**.       |
| 2008  | Aparece **GitHub**, desarrollado en Ruby on Rails.       |
| 2018  | **Microsoft compra GitHub**.                             |
| 2024  | Git domina el mercado (GitHub, GitLab, Bitbucket).       |

</details>

<details>
  <summary><strong>🧰 ¿Qué es Git?</strong></summary>

<p align="justify">
  <img align="right" src="https://leninmhs.com/wp-content/uploads/2023/11/git-historia.svg" width="100" style="margin-left: 15px; border-radius: 10px;" />

  <strong>Git</strong> es un sistema de control de versiones distribuido que permite trabajar con repositorios locales y remotos de forma eficiente y segura.
</p>


</details>


<details>
  <summary><strong>📁 ¿Qué es un Repositorio?</strong></summary>

Un **repositorio** es una carpeta que contiene:
- Las distintas versiones de los archivos.
- El historial completo de cambios.
Puede ser:
- 📍 **Local**: en tu máquina.  
- 🌐 **Remoto**: en un servidor (GitHub, GitLab, etc.).

</details>

<details>
  <summary><strong>🚀 Instalación de Git</strong></summary>

👉 Descarga Git desde: [https://git-scm.com/downloads](https://git-scm.com/downloads)

Pasos clave durante la instalación:

| Paso | Descripción | Imagen |
|------|-------------|--------|
| 1 | Selecciona la carpeta de destino | <img src="../Imagenes/Instalacion/paso1.png" width="200"/> |
| 2 | Selecciona todos los componentes | <img src="../Imagenes/Instalacion/paso2.png" width="200"/> |
| 3 | Agrega un acceso directo | <img src="../Imagenes/Instalacion/paso3.png" width="200"/> |
| 4 | Selecciona tu editor de texto | <img src="../Imagenes/Instalacion/paso4.png" width="200"/> |
| 5 | Rama principal: escribe `"main"` | <img src="../Imagenes/Instalacion/paso5.png" width="200"/> |
| 6 | Opción recomendada | <img src="../Imagenes/Instalacion/paso6.png" width="200"/> |
| 7 | Deja la opción SSH | <img src="../Imagenes/Instalacion/paso7.png" width="200"/> |
| 8 | Usa OpenSSL | <img src="../Imagenes/Instalacion/paso8.png" width="200"/> |
| 9 | Elige la primera opción (Unix: segunda) | <img src="../Imagenes/Instalacion/paso9.png" width="200"/> |
| 10 | Interfaz por defecto | <img src="../Imagenes/Instalacion/paso10.png" width="200"/> |
| 11 | Fast-Forward o merge | <img src="../Imagenes/Instalacion/paso11.png" width="200"/> |
| 12 | Deja por defecto | <img src="../Imagenes/Instalacion/paso12.png" width="200"/> |
| 13 | Activa caché de optimización | <img src="../Imagenes/Instalacion/paso13.png" width="200"/> |
| 14 | Clic en instalar | <img src="../Imagenes/Instalacion/paso14.png" width="200"/> |

</details>


<details>
  <summary><strong>📘 Primeros comandos en Git</strong></summary>

**Estos comandos te ayudarán a configurar Git una vez instalado. Suerte ❗❗❗**

| Nº | Comando                                               | Descripción breve                                      |
|----|--------------------------------------------------------|---------------------------------------------------------|
| 1  | `git --version`                                       | Verifica la versión de Git instalada                   |
| 2  | `git commit -am "mensaje"`                            | Hace commit y agrega cambios en archivos ya trackeados |
| 3  | `git help`                                            | Muestra ayuda general de Git                           |
| 4  | `git --help config`                                   | Muestra ayuda específica del comando `config`          |
| 5  | `git config --global user.name "Tu nombre"`           | Configura el nombre de usuario global                  |
| 6  | `git config --global user.email "Tu gmail"`           | Configura el correo global                             |
| 7  | `git config --global -e`                              | Abre el editor para configurar Git                     |
| 8  | `:wq`                                                 | Comando para guardar y salir (Vim/Nano)                |

</details>

<details>
  <summary><strong>📝 Notas y Recomendaciones</strong></summary>

<br/>

🔹 **Git vs GitHub**  
Git es el sistema de control de versiones que funciona en tu máquina local.  
GitHub es una plataforma en línea para almacenar repositorios Git y colaborar en equipo. ¡No son lo mismo!

---

🔹 **Buenas prácticas al usar Git:**

- 🔁 Realiza commits frecuentes y pequeños.  
- 🧠 Usa mensajes claros que expliquen qué hiciste.  
- 🚫 No subas archivos innecesarios (usa `.gitignore`).  
- 🛠️ Usa ramas para probar nuevas ideas sin afectar el código principal.  
- 📦 Documenta tu proyecto en el `README.md`.  

</details>


