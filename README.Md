# Backend API REST com Banco de Dados Fictício em JSON

Esta aplicação é um exemplo de um backend de API REST que utiliza um banco de dados fictício em JSON. A principal biblioteca empregada é o **json-server**, que permite simular um servidor RESTful de maneira simples e eficaz. Embora os dados sejam fictícios, esta aplicação oferece a capacidade de persistir informações, tornando-a uma ótima alternativa para aplicações em camadas onde o frontend é desenvolvido para consumir dados de uma fonte externa.

## Recursos Principais

- **API RESTful Simulada**: Através do json-server, você pode criar, ler, atualizar e excluir recursos de forma semelhante a uma API real. Isso torna a aplicação adequada para testar e desenvolver aplicações frontend sem depender de um servidor real.

- **Banco de Dados em JSON**: O banco de dados é representado por um arquivo JSON que contém dados fictícios. Mesmo que os dados não sejam reais, você pode interagir com eles como se fossem.

- **Persistência de Dados**: A aplicação permite que você persista dados fictícios, o que é útil para simulações e testes de casos de uso que requerem armazenamento temporário de informações.

## Como Usar

1. **Instalação**

   Certifique-se de que você tenha o [NodeJS](https://nodejs.org/en) e [json-server](https://github.com/typicode/json-server) instalado. Caso não tenha um dos dois, instale o NodeJS com o link acima e a dependência Json-Server na pasta do projeto com o seguinte comando:

   ```bash
   npm install --save json-server@0.13.0 -E

## Configurando o JSON-Server

Para evitar conflitos de porta com outras aplicações, é recomendável configurar o json-server para usar uma porta específica diferente da 3000. Siga os passos abaixo para configurar a porta:

1. Abra o arquivo `package.json` do seu projeto.

2. Na seção de "scripts", inclua um novo script de execução, por exemplo:

   ```json
   "scripts": {
     "start": "json-server --watch ./database/db.json --port 3001"
   }

3. Execute o comando: npm install (Para instalar os pacotes node_modules)

4. Agora, para iniciar o servidor json, execute o seguinte comando na raiz do seu projeto: npm start ou yarn start (Se você tiver o yarn como gerenciador de pacotes instalaldo)


## Info

Esse projeto possui um arquivo "db.json" com um array de usuários criado por mim na pasta database, você pode modificar ou excluir, se o JSON-Server não encontrar nenhum arquivo com base na diretiva do script/start, ele criará um e por padrão.

Agora você pode acessar a API REST simulada em http://localhost:3001 (ou a porta que você configurou). Utilize os endpoints para criar, ler, atualizar e excluir recursos como faria em uma API real.

Lembre-se de que os dados fictícios podem ser persistidos, o que significa que as alterações que você fizer serão refletidas nos dados armazenados no arquivo db.json.

## Exemplo de Uso

Para testar a funcionalidade da API, você pode fazer solicitações HTTP usando seu próprio projeto frontend, ferramentas como curl ou aplicativos como Postman.

Agora você está pronto para começar a utilizar este backend de API REST com banco de dados fictício em JSON para desenvolver e testar suas aplicações frontend. Divirta-se!

**Rafael Magno**