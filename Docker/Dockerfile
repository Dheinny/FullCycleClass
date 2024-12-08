# Defines a base for your image.
FROM nginx:latest

# Sets the working directory for any RUN, CMD, ENTRYPOINT, COPY, and ADD instructions that follow it in the Dockerfile.
# Diretorio criado na criacao da imagem e usado quando roda o container
WORKDIR /app    

# Executes any commands in a new layer on top of the current image and commits the result. RUN also has a shell form for running commands.
# Roda comando na imagem criada
RUN apt update && \
    apt install vim -y    

# COPY <src> <dest> Copies new files or directories from <src> and adds them to the filesystem of the container at the path <dest>.
# Copia arquivo do PC para o container
COPY nginx/html/ ./usr/share/nginx/html


# CMD <command>	Lets you define the default program that is run once you start the container based on this image.
#   Each Dockerfile only has one CMD, and only the last CMD instance is respected when multiple exist.
# Roda comando de entrada na inicialização do container