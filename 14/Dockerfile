# Usa a imagem base do Ubuntu
FROM ubuntu:22.04

# Instala Python e pip
RUN apt-get update && \
    apt-get install -y python3 python3-pip && \
    rm -rf /var/lib/apt/lists/*

# Instala pandas (opcional)
RUN pip3 install pandas

# Copia o script para o container
COPY process.py /app/process.py

# Define o diretório de trabalho
WORKDIR /app

# Comando padrão
CMD ["python3", "process.py"]