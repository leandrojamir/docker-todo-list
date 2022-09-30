# rode a partir da imagem do node na versão 14;
FROM node:14-alpine
# exponha a porta 3001;
EXPOSE 3001
# adicione o arquivo node_modules.tar.gz à imagem;
# Error response from daemon: dockerfile parse error line 6: ADD requires at least two arguments, but only one was provided. Destination could not be determined.
ADD node_modules.tar.gz ./docker/todo-app/back-end
# copie todos os arquivos da pasta back-end para a imagem. (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/back-end/Dockerfile);
# COPY ./docker/todo-app/back-end ./docker/todo-app/back-end/Dockerfile
# COPY failed: file not found in build context or excluded by .dockerignore: stat docker/todo-app/back-end: file does not exist
# -:11 DL3045 warning: `COPY` to a relative destination without `WORKDIR` set.
WORKDIR /todo-app/back-end
COPY . .
# inicie a aplicação com o comando npm start.
ENTRYPOINT ["npm", "start"]