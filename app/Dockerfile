# Usa una imagen base de Python
FROM python:3.9-slim

# Establece el directorio de trabajo en /app
WORKDIR /app

# Copia el archivo de requerimientos y luego instálalo
COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copia los archivos de la aplicación en el contenedor
COPY . .

# Expone el puerto en el que correrá Flask
EXPOSE 5000

# Define el comando para ejecutar la aplicación
CMD ["python", "app.py"]
