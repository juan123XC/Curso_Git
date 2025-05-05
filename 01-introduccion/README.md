<h2 align="center">
    01. Introducción a Git
  <img src="https://api.binarycoffee.dev/uploads/d196c5dabf39496c8c892f944d2102cf.jpg" width="60" style="vertical-align: middle; margin-left: 10px;">
</h2>

<details>
  <summary><h3 style="display: inline">🧠 ¿Qué es un Control de Versiones?</h3></summary>

Un **control de versiones** es un sistema que registra cada cambio realizado en los archivos de un proyecto.  
Permite:

- 📜 Llevar un historial completo de cambios.  
- 🧍 Saber *quién* hizo el cambio y *cuándo*.  
- 🔐 Mantener la seguridad y consistencia del código.  
- 🔄 Ofrece flexibilidad: no obliga a un desarrollo lineal.

</details>

<br/>

<details>
  <summary><h3 style="display: inline"> 📜 Breve Historia</h3></summary>

| Año   | Evento                                                    |
|-------|-----------------------------------------------------------|
| 1990  | Nace **CVS**, el primer sistema de control de versiones. |
| 2005  | Se crea **Git**, impulsado por **Linus Torvalds**.       |
| 2008  | Aparece **GitHub**, desarrollado en Ruby on Rails.       |
| 2018  | **Microsoft compra GitHub**.                             |
| 2024  | Git domina el mercado (GitHub, GitLab, Bitbucket).       |
</details>

<br/>

<details>
  <summary><h3 style="display: inline">🧰 ¿Qué es Git?</h3></summary>

**Git** es un sistema de control de versiones distribuido que permite trabajar con repositorios locales y remotos de forma eficiente y segura.

</details>

<br/>

<details>
  <summary><h3 style="display: inline">📁 ¿Qué es un Repositorio?</h3></summary>

Un **repositorio** es una carpeta que contiene:

- Las distintas versiones de los archivos.
- El historial completo de cambios.

Puede ser:

- 📍 **Local**: en tu máquina.
- 🌐 **Remoto**: en un servidor (GitHub, GitLab, etc.).
</details>

<br/>

<details>

  <summary><h3 style="display: inline">🚀 Instalación de Git (Haz clic para ver)</h3></summary>

👉 Descarga Git desde: [https://git-scm.com/downloads](https://git-scm.com/downloads)

Pasos clave durante la instalación:

1. Selecciona la carpeta de destino.

    <img src="../Imagenes/Instalacion/paso1.png" alt="Paso 1 - Instalación" width="300"/>
2. Seleccionar todo los componenetes

    <img src="../Imagenes/Instalacion/paso2.png" alt="Paso 1 - Instalación" width="300"/>
3. Agregar un shortcut del programa con el nombre Git.

    <img src="../Imagenes/Instalacion/paso3.png" alt="Paso 1 - Instalación" width="300"/>
4. Se debe agregar un IDE o neditor de texto como VIM NANO

    <img src="../Imagenes/Instalacion/paso4.png" alt="Paso 1 - Instalación" width="300"/>
5. Selecionamos Crear una rama por defecto Escribimos `"main"`

     <img src="../Imagenes/Instalacion/paso5.png" alt="Paso 1 - Instalación" width="300"/>
6. Selecionamos la opcion recomendada

    <img src="../Imagenes/Instalacion/paso6.png" alt="Paso 1 - Instalación" width="300"/>
7. Dejamos la opcion SSH

    <img src="../Imagenes/Instalacion/paso7.png" alt="Paso 1 - Instalación" width="300"/>
8. Dejamos el OpenSSL

    <img src="../Imagenes/Instalacion/paso8.png" alt="Paso 1 - Instalación" width="300"/>
9. Seleccionamos la primara opcion _Si tuvieramos Unix la segunda opcion_

     <img src="../Imagenes/Instalacion/paso9.png" alt="Paso 1 - Instalación" width="300"/>
10. Dejamos la interfaz predeterminada. 

    <img src="../Imagenes/Instalacion/paso10.png" alt="Paso 1 - Instalación" width="300"/>
11. Nos servira despues pero lo dejamos en Fast-Forward or merge.

    <img src="../Imagenes/Instalacion/paso11.png" alt="Paso 1 - Instalación" width="300"/>
12. Dejamos la opcion por defecto.

    <img src="../Imagenes/Instalacion/paso12.png" alt="Paso 1 - Instalación" width="300"/>
13. Habilitamos la primera opción para ejecutar algunos comandos más rápido debido a la caché.

    <img src="../Imagenes/Instalacion/paso13.png" alt="Paso 1 - Instalación" width="300"/>

14. No seleccionamos nada directamente install

    <img src="../Imagenes/Instalacion/paso14.png" alt="Paso 1 - Instalación" width="300"/>
---

</details>

<br/>

<details>
  <summary><h3 style="display: inline">📘 Primeros comandos en Git </h3></summary>

**Estos comandos te ayudaran a configurar tu Git una vez Instalado. Suerte ❗❗❗**

| Nº | Comando                                               | Descripción breve                                      |
|----|--------------------------------------------------------|---------------------------------------------------------|
| 1  | `git --version`                                       | Verifica la versión de Git instalada                   |
| 2  | `git commit -am "mensaje"`                            | Hace commit y agrega cambios en archivos ya trackeados |
| 3  | `git help`                                            | Muestra ayuda general de Git                           |
| 4  | `git --help config`                                   | Muestra ayuda específica del comando `config`          |
| 5  | `git config --global user.name "Tu nombre"`           | Configura el nombre de usuario global                  |
| 6  | `git config --global user.email "Tu gmail"`           | Configura el correo global              |
| 7  | `git config --global -e`                              | Abre el editor para configurar Git                    |
| 8  | `:wq`                                                 | Comando para guardar y salir en editores como Vim o Nano     |


</details>
