![logo header](logo_ADDE_header.png)

# Sobre a ADDE

Geramos valor ao negócio​ do nosso cliente através da criação de softwares.

Contamos com um time ​polivalente​ capaz de resolver os problemas do cliente de forma clara​ e organizada ​através do desenvolvimento de software.

Somos uma empresa jovem, funcionamos em ritmo de startup.

Ajudamos o cliente em todas as fases, desde a idealização​ do projeto até a entrega ​em produção.

# Resumo do desafio

Criar um sistema que mostre o clima atual e a previsão do tempo a partir do input de uma cidade e/ou localização do usuário.

# Histórias do usuário:
* Eu como usuário preciso de uma página Web que busque automaticamente a minha localização e me mostre os dados do clima atual
* Eu como usuário preciso que além do recurso de pegar automaticamente a minha localização no navegador, haja campo texto onde digito o nome de uma cidade para buscar os dados do clima atual
* Eu como usuário gostaria de poder ver a previsão do tempo para os próximos dias
* Eu como usuário gostaria de poder acessar a página tanto de um celular quanto de um computador
* Eu como usuário gostaria que a página apresentasse algum tipo de animação para diferentes tipos de clima, por exemplo uma nuvem cinza quanto o clima estiver nublado

## Requisitos

### Backend

* Criar um sistema que se comunique com uma api externa para pegar os dados de clima filtrado por cidade/região.
* Persistir o dados recuperados da API para serem utilizados como cache com tempo limite de 15 minutos.
* Tecnologia: Python 3 ([FastApi](https://fastapi.tiangolo.com/), [Flask](https://flask.palletsprojects.com/en/1.1.x/))

### Frontend

* Exibir os dados recuperados a partir do input do usuário. Por padrão, a previsão do tempo deverá ser baseada na localização atual do usuário.
* Tecnologia: [Angular](https://angular.io/) (>=8)

* Após consultar o clima, mostrar
  * Temperatura atual.
  * Cidade.
  * Clima (chovendo, nublado, ensolarado, etc).
  * Indicativo visual para mostrar o status do clima.

### Documentação

* Criar um README explicando um pouco das tecnologias usadas tanto no frontend quanto no backend
  * Um dev deve conseguir subir o seu projeto a partir do seu README
  * Para as APIs, sugerimos utilizar o SWAGGER


### Prazo

O prazo máximo para a entrega do teste será de **5 dias corridos** após o envio destas instruções.

## Forma de Entrega

Faça um repositório em alguma plataforma de controle de versão ([github](https://github.com), [gitlab](https://about.gitlab.com/), [bitbucket](https://bitbucket.org/), etc) contendo o projeto e nos mande o link notificando que a solução está entregue.

## Pontos extras que podem fazer a diferença

* Site responsivo.
* Testes unitários e integrados.
* Clean Code.
* Previsão do tempo para X dias.


## **Detalhes que farão diferença para DEVS Plenos**

* Utilizar o docker ou docker-compose para subir os projeto
  * Subir Backend
  * Subir Frontend
* Utilizar ferramentas de cache
  * Pode ser cache no próprio código ou algum banco de cache, por exemplo REDIS
* Realizar testes unitários e integrados nos sistemas
* Tratar erros no front caso haja falha de comunicação com o backend

## FAQ

>Posso utilizar bibliotecas externas?

Sim.

> Por que um Backend para consultar uma API externa?

 De modo geral, é mais interessante, pois, te dá mais controle e simplifica o consumo de vários clientes, exemplo: imagine que você tem vários consumidores requisitando essas API, um consumidor Web, um Android e um IOS. Caso você precise trocar a API que provém dados de clima, esta mudança será somente no backend e não nos clientes que a consomem. Além disso, queremos saber também se você pode lidar com uma API que consome uma ou várias APIs.

> E se o prazo estourar?

 Entregue o que você fez até aquele momento. Iremos analisar o seu trabalho.

> Que tipo de feedback terei?

 Se você tiver chance de seguir para uma segunda fase, entraremos em contato e te enviaremos um convite para um bate papo remoto. Caso você não seja aprovado nessa fase, te daremos o feedback por e-mail.

> Caso eu tiver alguma dúvida, poderei entrar em contato dentro deo prazo estipulado?

 Sim, se você tiver qualquer dúvida, sinta-se a vontade para entrar em contato conosco através do e-mail tecnologia@addesistemas.com.br

### Exemplos de APIs que podem ser utilizadas

* [Weatherbit](https://www.weatherbit.io/)
* [OpenWeatherMap](https://rapidapi.com/community/api/open-weather-map)
            [(exemplo de retorno)](http://api.openweathermap.org/data/2.5/weather?q=São%20paulo,br&lang=pt_br&units=metric&appid=aaa1129fc07f4aacb6763552a1f84c0b)

***
![logo footer](logo_ADDE_490x90.png)
