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

Instalar e executar o Backend

```
cd backend
npm install
npm start
```

Instalar e executar o Frontend

```
cd frontend
npm install
npm start
```

Instalar e executar o Mobile

Para testar a aplicação em um smartphone físico com Android, entre na Play Store e instale o app [Expo](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=pt_BR).

Edit o arquivo abaixo com o endereço IP do computador que esta executando o backend

```
mobile/src/services/api.js

import axios from 'axios';

const api = axios.create({
    baseURL: 'http://192.168.0.23:3333'
})

export default api;

```
cd mobile
npm install
```






And repeat

```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system

## Built With

* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

