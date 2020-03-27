# Be The Hero

Projeto construido durante a Semana OmniStack 11, promovido pela [RocketSeat ](https://rocketseat.com.br/week/inscricao/11.0). Foi construindo uma aplicação completa com Node.js no back-end, ReactJS no front-end e React Native no mobile.

O projeto se trata de uma aplicação para cadastro de ONG's de ajuda animais. Os pedidos de ajuda financeiro das ONG's são registrado como "caso".

O backend foi constriudo como uma API Rest para servi as aplicação da web e mobile.

Os registro das ONG's e seus casos são registrado na aplicação do frontend.

A aplicação mobile exibe todos os casos com a opção de envio de uma mensagem de e-mail ou WhatsApp para manisfestar interesse em fazer doação para a ONG. 

## Começando

Essas instruções fornecerão uma cópia do projeto em execução na sua máquina local para fins de desenvolvimento e teste.

### Requisitos

```
- git 2.20.1
- node v12.16.1
- npm 6.14.3
```

### Instalação

Exemplos passo a passo para criar um ambiente de desenvolvimento em execução

Primeiro clone o repositório do projeto.

```
git clone https://github.com/engmsilva/be-the-hero.git
```

Instale e execute o Backend

```
cd backend
npm install
npm start
```

Instale e execute o Frontend

```
cd frontend
npm install
npm start
```

Instale e execute o Mobile

Para testar a aplicação em um smartphone físico com Android, entre na Play Store e instale o app [Expo](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=pt_BR).

Edit o arquivo abaixo com o endereço IP do computador que esta executando o backend

```
mobile/src/services/api.js
```
```js
import axios from 'axios';

const api = axios.create({
    baseURL: 'http://192.168.0.23:3333'
})

export default api;

```
Execute o comando abaixo para iniciar e abrir a interface no navegado do Metro Bundler do Expo

```
cd mobile
npm install
npm start
```

Faça a leitura do QR code com a câmera do smartphone na página de interface do Metro Bundler do Expo.
O projeto deverá ser transferido para o smartpohe e o App executará automaticamente.


## Executando testes no Backend

Foram criados dois teste para exemplificar como são realizados os teste unitário e o teste de integração.

Os testes foram relizados usando a ferramenta Jest e Super Test.

O teste unitário foi aplicado em uma função que gera numeros rândomicos com uma quantidade de numeros conhecidos.

O teste de integração foi aplicado realizando uma requisição para a criação de um registro no banco de dados. Foi configurado uma banco de dados de teste separado do banco de dados da aplicação.

Comandos para executar o teste.
```
cd backend
npm install
npm test
```


