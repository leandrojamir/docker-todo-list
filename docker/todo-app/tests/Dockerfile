# rode a partir da imagem do mjgargani/puppeteer:trybe1.0;
FROM mjgargani/puppeteer:trybe1.0
# adicione o arquivo node_modules.tar.gz à imagem;
# unable to prepare context: path "/todo-app/tests" not found
WORKDIR /todo-app/tests
ADD node_modules.tar.gz ./
# copie todos os arquivos da pasta tests para a imagem. (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/tests/Dockerfile);
COPY . .
# inicie os testes com o comando npm test.
CMD ["npm", "test"]

