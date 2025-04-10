# Usa una imagen base oficial de Python
FROM python:3.9-slim

# Establece el directorio de trabajo
WORKDIR /app

# Copia los archivos necesarios
COPY code/python/requirements.txt .

# Instala las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Copia el resto del código
COPY code/python .

# Expone el puerto si tu app lo necesita (por ejemplo, FastAPI o Flask)
EXPOSE 8000

# Comando por defecto (ajústalo a lo que necesite tu app)
CMD ["python", "main.py"]
