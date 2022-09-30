# rode a partir da imagem do node na versão 14;
# testando com alpine mais "leve" para ver se não temporiza
#  10 - Gere uma build a partir do Dockerfile do `front-end` do `todo-app` nomeando a imagem para `todofrontend`
#     ✕ O avaliador deve executar o comando no arquivo 'command10.dc' (300006 ms)
#   11 - Gere uma build a partir do Dockerfile dos `testes` do `todo-app` nomeando a imagem para `todotests`
#     ✕ O avaliador deve executar o comando no arquivo 'command11.dc' (300002 ms)

FROM node:14-alpine
# exponha a porta 3000;
EXPOSE 3000
# adicione o arquivo node_modules.tar.gz à imagem;
ADD node_modules.tar.gz ./docker/todo-app/front-end
# copie todos os arquivos da pasta front-end para a imagem. (você pode usar o caminho relativo, lembrando que a Dockerfile está em ./docker/todo-app/front-end/Dockerfile);
WORKDIR /todo-app/front-end
COPY . .
# inicie a aplicação com o comando npm start.
ENTRYPOINT ["npm", "start"]
# ✕ O avaliador deve executar o comando no arquivo 'command10.dc' (300008 ms)
