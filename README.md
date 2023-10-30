# Whatsapp API Tutorial

Olá, este é um exemplo de implementação do [whatsapp-web.js](https://github.com/pedroslopez/whatsapp-web.js).

## Coisa Importante!

Como o WhatsApp faz atualizações regularmente, é necessário sempre usar a versão mais recente do whatsapp-web.js. Alguns erros podem ocorrer com versões antigas, portanto, tente atualizar a versão da biblioteca antes de criar um problema.

## Como Usar

1. Clone ou baixe este repositório.
2. Acesse o diretório do projeto.
3. Execute `npm install`.
4. Execute `npm run start:dev`.
5. Abra o navegador e vá para o endereço [http://localhost:8000](http://localhost:8000).
6. Leia o código QR.
7. Aproveite!

## Rodar em Segundo Plano
1. Instale o pm2 dentro da pasta `npm install pm2 -g`
2. Dentro da pasta do seu projeto inicie o serviço em pm2 `pm2 start app.js`

## Enviar Mensagem para um Grupo

Você pode enviar uma mensagem para qualquer grupo usando o chatID ou o nome do grupo. O chatID será usado se você especificar o campo `id` no formulário, então, se você quiser enviar pelo nome, use apenas o nome.

**Parâmetros:**

- `id` (opcional se o nome for fornecido): o ID do chat.
- `nome` (opcional): nome do grupo.
- `mensagem`: a mensagem.

Aqui está o endpoint: `/send-group-message`.

Para obter as informações dos grupos (incluindo ID e nome):

1. Envie uma mensagem para o número da API `!groups`.
2. A API responderá com as informações dos grupos.
3. Use o ID para enviar uma mensagem.
