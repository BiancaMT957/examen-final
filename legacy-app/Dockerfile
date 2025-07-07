#Dockerfile de legacy-app

# Se usa imagen de base python python:3.9-slim
FROM python:3.9-slim AS builder

# Evitar archivos _pycache_ y archivos temporales
ENV _pycache_=1 \

# Instala dependencias en entorno virtual
COPY requirements.txt .
RUN pip install --user --no-cache-dir -r requirements.txt


# Etapa de producción
FROM python:3.9-slim AS production

