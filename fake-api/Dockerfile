# Usar una imagen base de Python
FROM python:3.9-slim

# Establecer el directorio de trabajo
WORKDIR /usr/src/app

# Copiar el archivo de requisitos y la aplicación
COPY requirements.txt ./
#COPY main.py ./
COPY . .

# Instalar las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Exponer el puerto en el que la aplicación escuchará
EXPOSE 5000

# Comando para ejecutar la aplicación
CMD ["python", "main.py"]
