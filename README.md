# Pneumatic Sequence Analyzer (Cascade Method) ⚙️

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Status](https://img.shields.io/badge/Status-Active-success)

## 📖 Descripción General

Este proyecto es una herramienta de ingeniería desarrollada en Python para automatizar el cálculo y análisis de secuencias neumáticas utilizando el **Método Cascada**.

El programa procesa secuencias de movimiento complejas (incluyendo temporizadores), realiza la división lógica de grupos para evitar el bloqueo de señales (superposición), y genera automáticamente las tablas de verdad necesarias para el diseño del circuito de control neumático o electroneumático.

## 🚀 Funcionalidades Principales

* **Análisis Sintáctico de Secuencias:** Interpreta cadenas de texto con notación estándar (ej. `A+ B- C+[2s]`).
* **División Automática de Grupos:** Algoritmo que segmenta la secuencia basándose en la repetición de actuadores para minimizar el número de líneas de presión auxiliares.
* **Generación de Tablas de Lógica:**
    1.  **Tabla de Desarrollo:** Paso a paso del ciclo.
    2.  **Tabla de Grupos:** Lógica de conmutación de memorias/relés (Flip-Flops).
    3.  **Tabla de Movimientos:** Ecuaciones booleanas para la activación de solenoides.
* **Exportación:** Resultados presentados en DataFrames de Pandas para fácil lectura y exportación.

## 🛠️ Tecnologías

* **Python:** Lógica central y expresiones regulares (Regex).
* **Pandas:** Estructuración y presentación de datos tabulares.
* **Google Colab / Jupyter:** Entorno de ejecución interactivo.

## 📋 Ejemplo de Uso

Para una secuencia compleja como:
$$A- B- C+[2s] C- C+[2s] C- B+ A+$$

El sistema identificará automáticamente los 4 grupos de presión y generará la lógica de control, tal como se muestra en los ejercicios estándar de automatización industrial.

---
*Desarrollado como herramienta de apoyo para la asignatura de Automatización Industrial.*
