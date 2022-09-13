# rode a partir da imagem do node na versão 14;
FROM node:14
# exponha a porta 3000;
EXPOSE 3000
# adicione o arquivo node_modules.tar.gz à imagem;
ADD node_modules.tar.gz ./docker/todo-app/front-end
# copie todos os arquivos da pasta front-end para a imagem. (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/front-end/Dockerfile);
WORKDIR /todo-app/front-end
COPY . .
# inicie a aplicação com o comando npm start.
CMD ["npm", "test"]