
# Fundamentos de Algebra - Practica 1

## Información del Estudiante
- **Nombre:** Euruviel Márquez Martínez  
- **Matrícula:**  SW2509018
- **Grupo:** 1C 
- **Carrera:** TSW  
- **Cuatrimestre:** Primero  
- **Profesor:** Jorge Javier Pedrozo Romero  

# Actividad-21.-Cifrado-Hill



##  Descripción del Proyecto

Este repositorio contiene mi solución a la práctica de **Fundamentos de Programación**, donde implemento funciones en JavaScript para resolver problemas de álgebra básica, preparándome para trabajar con operaciones matriciales más complejas.

## 📌 Descripción del Proyecto

Este proyecto implementa un **encriptador y desencriptador basado en el
algoritmo Hill**, utilizando matrices **2×2** y operaciones módulo 26
para transformar mensajes en texto cifrado.

La aplicación:

-   Convierte el mensaje en una matriz numérica basada en el alfabeto.
-   Permite ingresar una matriz clave 2×2.
-   Encripta el mensaje usando multiplicación matricial mod 26.
-   Desencripta el mensaje utilizando la matriz inversa módulo 26.
-   Incluye una interfaz visual desarrollada en HTML, CSS y JavaScript.

------------------------------------------------------------------------

## 🚀 Instrucciones de Uso


------------------------------------------------------------------------

### 2️⃣ Ingresar el mensaje

-   Escribir un mensaje de máximo **30 caracteres**.\
-   Todo se convierte a **mayúsculas** automáticamente.
-   Solo se aceptan letras A--Z.

------------------------------------------------------------------------

### 3️⃣ Ingresar la matriz clave 2×2

    | a  b |
    | c  d |

Ejemplo:

    3   3
    2   5

Debe ser **invertible módulo 26**.

------------------------------------------------------------------------

### 4️⃣ Encriptar

Haz clic en **Encriptar**.

------------------------------------------------------------------------

### 5 Desencriptar

Haz **doble clic** sobre el texto encriptado.

------------------------------------------------------------------------

##  Matemáticas del Algoritmo

###  Representación del alfabeto

A=0, B=1, ..., Z=25.

------------------------------------------------------------------------

### 🔢 División en pares

Ejemplo:

    H O → [7,14]
    L A → [11,0]

Si falta un caracter, se agrega **X (23)**.

------------------------------------------------------------------------

### 🔐 Encriptación

\[ C = K `\cdot `{=tex}V `\mod 26`{=tex} \]

------------------------------------------------------------------------

### 🔓 Condición de clave válida

\[ `\det`{=tex}(K) = ad - bc \] Debe cumplir: \[
`\gcd`{=tex}(`\det`{=tex}(K), 26) = 1 \]

------------------------------------------------------------------------

### 🔁 Matriz inversa módulo 26

\[ K\^{-1} = (`\det`{=tex}(K)\^{-1} `\mod 26`{=tex}) egin{bmatrix} d &
-b\
-c & a \\end{bmatrix} `\mod 26`{=tex} \]

------------------------------------------------------------------------

### 🔍 Desencriptación

\[ V = K\^{-1} `\cdot `{=tex}C `\mod 26`{=tex} \]

------------------------------------------------------------------------
