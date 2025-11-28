# PLANTAS-VENENOSAS
# 🌿 CLASIFICADOR DE PLANTAS VENENOSAS (TEACHABLE MACHINE)

## 💡 Descripción del Proyecto

Este proyecto es una aplicación web sencilla que utiliza un modelo de **Machine Learning (Aprendizaje Automático)**, entrenado con **Google Teachable Machine**, para clasificar imágenes en tiempo real.

El modelo está diseñado para identificar las siguientes clases de plantas:

* Adelfa
* Dieffenbachia
* Hiedra venenosa
* [Y las otras 7 clases que entrenaste, ej: Belladona, Ricino, etc.]

## ⚙️ Tecnologías y Librerías

* **Modelo de Clasificación:** Teachable Machine (Clasificación de Imágenes).
* **Framework ML:** TensorFlow.js (para ejecutar el modelo en el navegador).
* **Lenguajes:** HTML y JavaScript.

## 🚀 Instrucciones de Ejecución

Para ejecutar esta aplicación, es **fundamental** usar un servidor local para que el navegador cargue correctamente el modelo de Machine Learning sin restricciones de seguridad.

1.  **Descarga/Clona el Repositorio:** Asegúrate de tener todos los archivos (incluyendo `index.html`, `model.json`, `metadata.json` y `weights.bin`) en una carpeta local.
2.  **Instala un Servidor Local:**
    * **Opción Recomendada (VS Code):** Si usas Visual Studio Code, instala la extensión **"Live Server"** de Ritwick Dey.
    * **Opción Alternativa (Python):** Si tienes Python instalado, puedes abrir la terminal en la carpeta del proyecto y ejecutar: `python -m http.server`.
3.  **Abre la Aplicación:**
    * Si usas **Live Server**, haz clic derecho en `index.html` y selecciona **"Open with Live Server"**.
    * Si usas Python, abre tu navegador y ve a la dirección **`http://localhost:8000`** (o el puerto que te indique la terminal).
4.  **Uso:** Haz clic en el botón **"Start"** y autoriza el acceso a la cámara web. El modelo comenzará a clasificar la imagen en tiempo real.

---

##  troubleshooting (Solución de Problemas)

Si la aplicación no funciona o el modelo no carga:

* **Problema Común:** Si abres el archivo con doble clic (`file:///...`), el navegador bloqueará la carga del modelo por seguridad. **La solución es usar el servidor local (Paso 2).** 
* **Rutas del Modelo:** Confirma que el código en el archivo `index.html` use la ruta correcta para buscar los archivos: `const URL = "./";`
