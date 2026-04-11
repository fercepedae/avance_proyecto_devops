# 🚀 Proyecto DevOps - Soluciones Tecnológicas del Futuro

Este proyecto implementa una arquitectura DevOps en AWS utilizando prácticas modernas de automatización, integración continua y despliegue continuo (CI/CD), con el objetivo de mejorar la entrega de software, reducir errores manuales y optimizar la infraestructura en la nube.

---

## 🧠 Objetivo

Automatizar el despliegue de una aplicación web en AWS utilizando herramientas de DevOps como GitHub Actions, Docker, EC2 y scripts de automatización, mejorando la eficiencia del proceso de entrega.

---

## 🏗️ Arquitectura

- Repositorio en GitHub
- CI/CD con GitHub Actions
- Servidor EC2 en AWS
- Contenedores Docker
- Monitoreo con AWS CloudWatch
- Automatización con Boto3
- Infraestructura como código con CloudFormation

---

## ⚙️ Tecnologías utilizadas

- AWS EC2
- AWS CloudWatch
- AWS CloudFormation
- Docker
- Docker Compose
- GitHub Actions
- Git
- Python (Boto3)
- Linux (Ubuntu)
- Bash scripting

---

## 🚀 CI/CD Pipeline

El pipeline automatiza:

1. Checkout del código desde GitHub
2. Construcción de imagen Docker
3. Conexión SSH a EC2
4. Pull del repositorio en el servidor
5. Detención y eliminación del contenedor anterior
6. Construcción y ejecución del nuevo contenedor

---

## 🐳 Docker

La aplicación se ejecuta en un contenedor Nginx que sirve un archivo `index.html`.

### Ejecutar localmente:

```bash
docker build -t app .
docker run -d -p 80:80 app
