# rode a partir da imagem do mjgargani/puppeteer:trybe1.0;
FROM mjgargani/puppeteer:trybe1.0
# adicione o arquivo node_modules.tar.gz à imagem;
# unable to prepare context: path "/todo-app/tests" not found
ADD node_modules.tar.gz ./docker/todo-app/tests
# copie todos os arquivos da pasta tests para a imagem. (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/tests/Dockerfile);
WORKDIR /todo-app/tests
COPY . .
# inicie os testes com o comando npm test.
CMD ["npm", "test"]

