# Event-Driven Architecture to Improve Performance and Scalability in Microservices-Based Systems

Rahmatulloh, Alam & Nugraha, Fuji & Gunawan, Rohmat & Darmawan, Irfan. (2022). Event-Driven Architecture to Improve Performance and Scalability in Microservices-Based Systems. 01-06. 10.1109/ICADEIS56544.2022.10037390. 

## 1. Fichamento de Conteúdo

O artigo investiga a aplicação da Arquitetura Orientada a Eventos (EDA) para melhorar o desempenho e a escalabilidade em sistemas baseados em microservices. Os autores partem do problema de que a comunicação síncrona via HTTP (API-Driven) entre microservices pode prejudicar o desempenho e a escalabilidade do sistema. Como solução, propõem a integração de tecnologia de containers (Docker e Kubernetes) com EDA para lidar com a comunicação interna de forma assíncrona. O estudo implementa um sistema de exemplo para uma loja de tecidos, composto por quatro serviços principais (Auth, Cloth, Stock, Sale) e um barramento de eventos (NATS Streaming). Através de uma metodologia experimental que compara a EDA com a abordagem API-Driven, os resultados mostram que a EDA obteve um tempo de resposta 19.18% mais rápido e uma taxa de erro 34.40% menor, embora tenha consumido 8.52% mais CPU. Conclui-se que a EDA, combinada com orquestração de containers, é uma abordagem viável para melhorar a escalabilidade e o desempenho em arquiteturas de microservices, apesar do maior consumo de recursos computacionais.

## 2. Fichamento Bibliográfico

* _Arquitetura Orientada a Eventos (Event-Driven Architecture - EDA)_: Padrão arquitetural onde serviços fracamente acoplados trocam informações de forma assíncrona através da publicação e escuta de eventos, contrastando com a comunicação síncrona baseada em chamadas de API (API-Driven) (página 3).
* _Tecnologia de Containers_: Sistemas operacionais leves que abstraem a aplicação e suas dependências do SO hospedeiro, proporcionando portabilidade e facilitando o deployment e escalabilidade de microservices. Docker e Kubernetes são tecnologias-chave nesta abordagem (página 3).
* _Tempo de Resposta (Response Time)_: Métrica de desempenho medida em milissegundos, representando o tempo entre o envio de uma requisição pelo cliente e o recebimento da resposta. Uma métrica crítica para Acordos de Nível de Serviço (SLAs) (página 4).
* _Taxa de Erro (Error Rate)_: Métrica que expressa, em porcentagem, a quantidade de requisições que falham ou não são processadas dentro de um período de tempo definido (ramp-up period), indicando a robustez do sistema sob carga (página 4).
* _NATS Streaming_: Tecnologia utilizada como barramento de eventos (event-bus) no estudo, responsável por gerir a comunicação assíncrona de publish/subscribe entre os microservices (página 4).

## 3. Fichamento de Citações

*  _"Synchronous HTTP communication is a communication that is usually done by microservices with an API-driven architecture (API-Driven Architecture) "_
*  _"Event-Driven can be applied as a way of communicating between microservices, when there is a large volume of data that needs to be processed and when no response is expected "_
*  _"EDA allows information to be absorbed into an event-driven ecosystem and then broadcast to the listening service or the service that will receive the event "_
*  _"From the measurement results, it is known that the performance of the Event-Driven Architecture is better than the API-Driven Architecture "_
*  _"Event-Driven Architecture response time is faster with a percentage increase of 19.18%, the error rate of Event-Driven Architecture is lower with a percentage increase of 34.40%, although CPU usage Event-Driven Architecture is higher with a percentage decrease of 8.52%. "_