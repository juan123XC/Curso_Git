
# 01. Introducción a Git


<details>
  <summary><strong>🧠 ¿Qué es un Control de Versiones?</strong></summary>

Un **control de versiones** es un sistema que registra cada cambio realizado en los archivos de un proyecto.  
Permite:

- 📜 Llevar un historial completo de cambios.  
- 🧍 Saber *quién* hizo el cambio y *cuándo*.  
- 🔐 Mantener la seguridad y consistencia del código.  
- 🔄 Ofrece flexibilidad: no obliga a un desarrollo lineal.

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

**Git** es un sistema de control de versiones distribuido que permite trabajar con repositorios locales y remotos de forma eficiente y segura.

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
  <summary><strong>🚀 Instalación de Git (Haz clic para ver)</strong></summary>

👉 Descarga Git desde: [https://git-scm.com/downloads](https://git-scm.com/downloads)

Pasos clave durante la instalación:

1. Selecciona la carpeta de destino.
    ![](../Imagenes/Instalacion/paso1.png)
2. Selecciona todos los componentes.  
    ![](../Imagenes/Instalacion/paso2.png)
3. Agrega un acceso directo.  
    ![](../Imagenes/Instalacion/paso3.png)
4. Selecciona tu editor de texto.  
    ![](../Imagenes/Instalacion/paso4.png)
5. Rama principal: escribe `"main"`  
    ![](../Imagenes/Instalacion/paso5.png)
6. Opción recomendada  
    ![](../Imagenes/Instalacion/paso6.png)
7. Deja la opción SSH  
    ![](../Imagenes/Instalacion/paso7.png)
8. Usa OpenSSL  
    ![](../Imagenes/Instalacion/paso8.png)
9. Elige la primera opción (Unix: segunda)  
    ![](../Imagenes/Instalacion/paso9.png)
10. Interfaz por defecto  
    ![](../Imagenes/Instalacion/paso10.png)
11. Fast-Forward o merge  
    ![](../Imagenes/Instalacion/paso11.png)
12. Deja por defecto  
    ![](../Imagenes/Instalacion/paso12.png)
13. Activa caché de optimización  
    ![](../Imagenes/Instalacion/paso13.png)
14. Clic en instalar  
    ![](../Imagenes/Instalacion/paso14.png)

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

