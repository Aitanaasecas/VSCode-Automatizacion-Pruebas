VSCode-Automatizacion-Pruebas
Como usar VSCODE orientado a pruebas automatizadas

**

Introducción
**

Este repositorio tiene como objetivo explicar el funcionamiento de Visual Studio Code (VS Code) orientado a la automatización de pruebas. Aquí encontrarás información sobre su instalación, configuración, extensiones útiles y ejemplos prácticos para pruebas con herramientas como PyTest y Selenium.

Instalación de VS Code

Descarga VS Code desde la página oficial.
(https://code.visualstudio.com/)

Instálalo siguiendo las instrucciones de tu sistema operativo.

Abre VS Code y personaliza la interfaz según tus preferencias.

Extensiones Recomendadas

Para mejorar la experiencia en automatización de pruebas, instala las siguientes extensiones:

Python (Microsoft): Soporte para desarrollo en Python.

Pylance: Autocompletado y análisis de código.

Test Explorer UI: Ejecución y visualización de pruebas automatizadas.

Selenium IDE (Opcional): Herramientas para pruebas en navegadores.

GitLens: Integración con Git para control de versiones.

Configuración de Git en VS Code

Instala Git en tu sistema y verifica la instalación con:

git --version
Configura tu usuario:

git config --global user.name "TuNombre"
git config --global user.email "tuemail@example.com"
Clona un repositorio o crea uno nuevo en GitHub y conéctalo con VS Code.

Ejemplos de Automatización de Pruebas

Prueba con PyTest

Instala PyTest:

pip install pytest
Crea un archivo test_sample.py con el siguiente contenido:

def suma(a, b):
    return a + b

def test_suma():
    assert suma(2, 3) == 5
Ejecuta la prueba en la terminal:

pytest test_sample.py
Prueba con Selenium

Instala Selenium:

pip install selenium
Crea un archivo test_selenium.py con el siguiente código:

from selenium import webdriver

driver = webdriver.Chrome()
driver.get("https://www.google.com")
print(driver.title)
driver.quit()
Ejecuta el script con:

python test_selenium.py
Contribuciones

Si quieres mejorar este repositorio, siéntete libre de hacer un fork y enviar tus mejoras mediante pull requests.

Recursos Adicionales

Documentación oficial de VS Code

Guía de Git y GitHub

PyTest

Selenium
