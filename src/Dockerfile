#não sabia como puxar o postgres pra dentro do projeto, ou se devia fazer um docker run para 
#para um container postgres em separado; por fim optei por chamar a imagem dentro do docker file
# e sem atribuir as variáveis de banco aqui, mas dentro do yaml
FROM postgres
FROM node
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY ..
EXPOSE 8080
CMD ["node","server.js"]
