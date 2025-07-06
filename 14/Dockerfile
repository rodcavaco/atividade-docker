# Usa imagem base do Ubuntu
FROM ubuntu:22.04

# Evita prompts interativos na instalação
ENV DEBIAN_FRONTEND=noninteractive

# Atualiza o sistema e instala o Python
RUN apt-get update && \
    apt-get install -y python3 && \
    apt-get clean

# Cria diretório de trabalho
WORKDIR /app

# Copia o script para o container
COPY process.py .

# Define o comando padrão para rodar o script
CMD ["python3", "process.py"]
