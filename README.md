# Laboratorio: Integracion de IA Local, Redes y Ciberseguridad (Ubuntu / Ollama)

Repositorio de entregables para el laboratorio practico de despliegue de modelos de lenguaje locales, administracion de servicios en Linux y analisis de trafico de red.

## Integrante
* Juan Gomez

---

## Tecnologias y Herramientas Utilizadas
* Sistema Operativo: Ubuntu (via Oracle VirtualBox en hardware Lenovo LOQ).
* Motor de IA: Ollama (ejecutando un modelo local de ciberseguridad).
* Desarrollo Web: HTML5 y JavaScript (API REST / fetch).
* Analisis de Redes: Wireshark y comandos de red nativos (SSH/TCP).
* Control de Versiones: Git y GitHub.

---

## Estructura del Repositorio
* `INFORME JUAN GÓMEZ (1).pdf`: Informe del paso a paso de la realización del taller y proyecto.
* `index.html`: Interfaz web interactiva para la consulta del modelo local con gestion de errores y diseno responsivo.
* `Modelfile`: Archivo de configuracion del modelo personalizado en Ollama.
* `README.md`: Documentacion y guia del proyecto.

---

## Instrucciones de Ejecucion

### 1. Iniciar el servicio de IA local (Ollama)
Configura el host y los origenes para permitir la comunicacion con el entorno de red:
```bash
sudo -u ollama env OLLAMA_HOST="0.0.0.0" OLLAMA_ORIGINS="*" ollama serve
```

### 2. Levantar la interfaz web
En una nueva pestana de la terminal, navega hasta la carpeta del proyecto e inicia un servidor HTTP local:
```bash
python3 -m http.server 8000
```

### 3. Acceso
Abre tu navegador web e ingresa a:
```text
http://localhost:8000
```
