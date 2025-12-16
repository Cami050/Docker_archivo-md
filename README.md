# Informe Tecnico Docker 
# 🐳 Informe Técnico – Docker  
**Autora:** Camila Rivera  
**Fecha:** Noviembre 2025  

---

##  Resumen del Video 1 – Introducción a Docker  

Docker permite **desarrollar en equipo dentro de un entorno controlado y uniforme**, reduciendo errores (“bugs”) ocasionados por diferencias de configuración entre equipos.  
Facilita la **instalación rápida de dependencias**, el **empaquetado de aplicaciones** y un **despliegue a producción más simple y confiable**.

###  Concepto de contenedores  
Los contenedores permiten **empaquetar una aplicación junto con todas sus dependencias, archivos de configuración y entorno necesario**.  
Por ejemplo, un contenedor puede incluir:
- Código fuente (HTML, Node.js, Python, etc.)  
- Archivo `.env` con variables de entorno  
- Librerías, frameworks y configuraciones específicas  

Este empaquetado hace que el contenedor sea **portable**, lo que significa que puede ejecutarse en cualquier máquina con Docker instalado.  
Así se logra un desarrollo y despliegue **más coherente, rápido y reproducible**.

###  Almacenamiento de imágenes  
Los contenedores se basan en **imágenes**, almacenadas en repositorios de contenedores (públicos o privados).  
Ejemplo: **Docker Hub**, donde existen imágenes oficiales de tecnologías como Node.js, Python, MySQL, PostgreSQL, Golang o Linux Alpine.

###  Antes de Docker  
Antes, los desarrolladores trabajaban en distintos sistemas operativos y versiones de herramientas (por ejemplo, versiones diferentes de Node.js).  
Esto generaba incompatibilidades y pérdida de tiempo.  
Con Docker, todos trabajan sobre una **misma imagen**, eliminando esos conflictos y acelerando el desarrollo.

###  Despliegue y automatización  
Sin contenedores, los errores eran frecuentes por versiones distintas de dependencias.  
Con Docker, se usan imágenes reproducibles y pipelines automatizados (CI/CD) que hacen el despliegue casi automático.

###  Imágenes y contenedores  
- **Imagen:** empaquetado con el código, dependencias y configuraciones.  
- **Contenedor:** instancia ejecutable de una imagen.  

Los contenedores se construyen en **capas** (base Linux, dependencias, aplicación).  
Gracias a esto son **ligeros y rápidos**, mucho más que las máquinas virtuales tradicionales.

###  Docker y virtualización  
Docker usa **virtualización a nivel de sistema operativo**, compartiendo el kernel del anfitrión.  
Por eso las imágenes son mucho más livianas y eficientes.  

**Tipos de virtualización:**  
1. Paravirtualización (cada VM tiene su propio sistema operativo).  
2. Virtualización parcial.  
3. Virtualización completa (todo se virtualiza).  

Docker es superior porque **usa directamente el kernel del host**, reduciendo el consumo de recursos.

---

##  Resumen del Video 2 – Docker de Novato a Pro  

El segundo video explica cómo **Docker simplifica el flujo completo de desarrollo**, desde construir imágenes hasta ejecutar servicios complejos.  

###  Conceptos principales:  
- **Dockerfile:** archivo con instrucciones para construir una imagen personalizada.  
- **Docker Build:** comando que crea una imagen según el Dockerfile.  
- **Docker Run:** ejecuta un contenedor a partir de una imagen.  
- **Docker Compose:** herramienta para ejecutar varios contenedores (por ejemplo, aplicación + base de datos).  
- **Docker Hub:** plataforma para publicar y descargar imágenes.  
- **Volúmenes:** permiten guardar datos fuera del contenedor (persistencia).  
- **Puertos:** conectan el contenedor con el exterior (`-p 3000:3000`).  

###  Casos prácticos mostrados  
- Crear un contenedor con una app web Node.js.  
- Ejecutar una base de datos MySQL en otro contenedor.  
- Conectarlos con `docker-compose.yml` para simular un entorno real.  
- Personalizar imágenes con dependencias y versiones específicas.  

###  Flujo típico de trabajo  
1. Crear `Dockerfile`.  
2. Construir imagen con `docker build`.  
3. Ejecutar contenedor con `docker run`.  
4. Orquestar varios servicios con `docker-compose`.  
5. Publicar imagen en Docker Hub o en un registro privado.  

---

##  Reflexiones personales  

###  **Ventajas:**  
- Entornos idénticos para todo el equipo.  
- Reducción de errores por versiones diferentes.  
- Despliegues a producción más rápidos.  
- Fácil integración con pipelines CI/CD.  
- Portabilidad total: *“funciona igual en mi máquina y en la tuya”*.

###  **Desafíos:**  
- Curva inicial de aprendizaje.  
- Configuración de redes y volúmenes puede ser confusa.  
- Requiere planificación para la seguridad y el tamaño de imágenes.  

###  **Uso práctico:**  
Docker es ideal para estudiantes, desarrolladores y empresas que quieran **automatizar despliegues**, **mantener entornos controlados** y **probar software en múltiples plataformas** sin conflictos de dependencias.

---

##  Ejemplo práctico – Mini Proyecto con Docker  

Este proyecto crea un **servidor web básico en Node.js** dentro de un contenedor.  

###  Estructura
## 6. Evidencias del proyecto

A continuación se muestran algunos pantallazos del funcionamiento del contenedor:

**Construcción de la imagen**
![Build del contenedor](imagenes/1.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/2.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/3.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/4.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/5.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/6.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/7.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/8.jpg)

**Ejecución del contenedor**
![Contenedor ejecutándose](imagenes/9.jpg)



**Enlaces Git** https://github.com/Cami050/Docker2_CR   
**Enlaces Docker** https://github.com/Cami050/Docker2_CR