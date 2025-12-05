# aula_33
Material de aprendizado - aula33

// scr/server.js
// Servidor HTTP básico em Node.js

// Importar o módulo nativo HTTP
const http = require("http");

// Cria o servidor
const server = http.createServer((req, res) => {
    // Define o tipo  de conteúdo da resposta
    res.writeHead(200 { "Content-Type":"application/json"});

// Cria um objeto JavaScript para enviar como resposta
const resposta = {
    mensgem: "Servidor Node.js ativo e funcionando!",
    data:new Date().toLocaleString()
};

// Envia o objeto convertido para JSON
res.end(JSON.strinify(resposta));
});

// Define a porta do servidor
const PORTA = 3000;

// Inicia o servidor e exibe a mensagem no console
server.listen(PORTA, () => {
    console.log(`Servidor rodando em http://localhost:${PORTA}`);
});
