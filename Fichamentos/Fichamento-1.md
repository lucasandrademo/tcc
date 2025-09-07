# Event-Driven Architecture (EDA) vs API-Driven Architecture (ADA): Which Performs Better in Microservices?

A. Rahmatulloh, F. Nugraha, R. Gunawan, I. Darmawan, E. Haerani and R. Rizal, "Event-Driven Architecture (EDA) vs API-Driven Architecture (ADA): Which Performs Better in Microservices?," 2024 International Conference on Artificial Intelligence, Blockchain, Cloud Computing, and Data Analytics (ICoABCD), Indonesia, 2024, pp. 31-36, doi: 10.1109/ICoABCD63526.2024.10704326.

## 1. Fichamento de Conteúdo

O artigo compara o desempenho de duas arquiteturas de comunicação em microsserviços: a arquitetura orientada a eventos (Event-Driven Architecture - EDA) e a arquitetura orientada a APIs (API-Driven Architecture - ADA). Os autores argumentam que, embora a arquitetura de microsserviços seja amplamente adotada para substituir monólitos, a comunicação síncrona baseada em HTTP (ADA) pode prejudicar o desempenho à medida que o número de serviços aumenta. A solução proposta é o uso de comunicação assíncrona baseada em eventos (EDA) combinada com tecnologia de contêineres para melhorar a escalabilidade. O estudo implementa um protótipo com quatro serviços (autenticação, tecidos, estoque e vendas) e mede três parâmetros: tempo de resposta, taxa de erro e uso de CPU. Os resultados mostram que a EDA supera significativamente a ADA, com redução de 30% no tempo de resposta, 7% na taxa de erro e 4% no uso de CPU. Conclui-se que a EDA é mais eficiente em ambientes de microsserviços com alta concorrência.

## 2. Fichamento Bibliográfico 

* _Event-Driven Architecture (EDA)_ é um estilo arquitetural baseado em eventos, onde os serviços comunicam-se de forma assíncrona por meio de publicação e escuta de eventos, utilizando um barramento de eventos como intermediário (página 2).
* _API-Driven Architecture (ADA)_ é uma abordagem de comunicação síncrona entre microsserviços, baseada em chamadas HTTP e APIs, onde o cliente aguarda uma resposta direta do servidor (página 1).
* _Microservices_ referem-se a um conjunto de serviços independentes que se comunicam para formar uma aplicação complexa, permitindo flexibilidade no desenvolvimento e uso de diferentes tecnologias por serviço (página 2).
* _Container Technology_ é uma forma de virtualização leve que encapsula aplicações e suas dependências, facilitando a implantação, escalabilidade e portabilidade entre diferentes ambientes (página 2).
* _NATS Streaming_ é uma tecnologia de barramento de eventos utilizada para implementar a comunicação assíncrona entre serviços no padrão publish-subscribe (página 3).


## 3. Fichamento de Citações

* _"Microservice architecture is increasingly used because it offers high flexibility, can adapt to technological changes, and can help simplify developers' work."_
* _"HTTP synchronous communication is usually used in microservices with API-Driven Architecture (ADA)."_
* _"Event-driven architecture (EDA) works based on events, event publishing, and listening exchange of information or data."_
* _"The experimental findings in this study indicate that the response time of microservice architecture for EDA-Driven data communication is 30% faster than ADA-Driven data communication."_
* _"There was a decrease in error rate of about 7% and a decrease in CPU usage of about 4% when EDA-Driven data communication was implemented in microservice architectures, compared to ADA-Driven data communication."_
* _"EDA can provide advantages in developing distributed systems that are more flexible and have high concurrency."_