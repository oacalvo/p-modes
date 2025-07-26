# 🌞 p-modes: Filtrado de modos p con redes neuronales

Este proyecto explora el uso de redes neuronales para intentar filtrar los modos p solares (p-modes) a partir de observaciones del SDO continuo. Aunque los resultados no fueron  satisfactorios, el trabajo representa un primer acercamiento al uso de aprendizaje automático para replicar técnicas clásicas de filtrado en datos solares.

## 📁 Contenido del repositorio

El repositorio contiene tres archivos principales:

- 🌀 `resultados.gif`: Visualización del cubo predicho por la red neuronal.
- 📄 `metodologia.pdf`: Documento que describe el método de entrenamiento y las pruebas realizadas.
- 🧠 `modelo_p_modes.ipynb`: Notebook ejecutable en Google Colab que permite montar Google Drive, cargar los cubos y ejecutar la red neuronal.

> **Nota:** Debido al tamaño de los archivos (~GB), los tres cubos utilizados en el entrenamiento **no están incluidos** en este repositorio:
>
> - Cubo original sin filtrar  
> - Cubo filtrado con método clásico (Fourier)  
> - Cubo predicho por la red neuronal

Estos deben almacenarse en tu Google Drive personal y vincularse desde Colab para su ejecución. Pero estan todos los codigos de descarga para que cada persona pueda hacer el tratamiento de imágenes

## ⚙️ Estructura del código

El notebook se divide en dos secciones principales:

1. **Red neuronal principal:** corresponde al modelo reportado en el PDF, con resultados concretos.
2. **Pruebas adicionales:** incluye varios intentos fallidos o experimentales con diferentes arquitecturas, activaciones y estrategias de entrada (por ejemplo, uso de ventanas espaciales).

## 🔬 Objetivo

El objetivo general fue evaluar si una red neuronal puede aprender a replicar el filtrado de modos p aplicado clásicamente en el espacio k-omega, utilizando datos de intensidad.

## 📌 Observaciones

- El modelo fue entrenado tomando como entrada la serie temporal de un único píxel, lo cual limitó su capacidad para capturar coherencia espacial.
- Se proponen futuras mejoras utilizando ventanas espacio-temporales o redes convolucionales 2D/3D en el espacio de Fourier.

---

✍️ *Este trabajo fue realizado por Óscar Calvo*
