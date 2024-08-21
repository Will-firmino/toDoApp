# Comandos úteis do Angular

npm i -g @angular/cli -> Comando para instalar o angular;
ng v -> Verificar se o Angular está instalado e qual a versão que está configurada;
ng new ToDoApp -> Comandor para gerar um novo App;
ng serve -> Inicializa o servidor;
ng generate component components/cabecalho -> Criar um novo componente
ng g c components/cabecalho -> Criar um novo componente com o g compacto.

===============================================================================
# Criando uma API simples

## Instalação de uma API simples
1. Criar uma pasta backend;
2. Na pasta backend, iremos abrir o terminal e rodar o comando `npm init -y`
para que seja instalado o arquivo [package.json].
3. Será criado um arquivo [package.json].
4. Iremos criar um arquivo chamado [db.json] dentro da pasta backend.
5. Dentro do arquivo [package.json], em scripts, alterar de para:
de:
```json
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  } 
para:

"scripts": {
    "start": "json-server --watch db.json --port 3301"
  },
```

6. Agora, precisamos instalar a depêndencia json-server, rodando no terminal o comando `npm install json-server`;
7. Agora, iremos rodar o nosso servidor backend utilizando o comando `npm start`;