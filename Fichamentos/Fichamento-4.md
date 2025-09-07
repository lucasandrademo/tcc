# Performance Analysis of Microservice Design Patterns

A. Akbulut and H. G. Perros, "Performance Analysis of Microservice Design Patterns," in IEEE Internet Computing, vol. 23, no. 6, pp. 19-27, 1 Nov.-Dec. 2019, doi: 10.1109/MIC.2019.2951094.

## 1. Fichamento de Conteúdo

O artigo realiza uma análise de desempenho de três padrões de design de microservices amplamente utilizados na indústria: API Gateway, Cadeia de Responsabilidade (Chain of Responsibility) e Mensageria Assíncrona. O objetivo principal é avaliar o desempenho desses padrões em termos de tempo de resposta de consulta, uso eficiente de hardware, custos de hospedagem e taxa de perda de pacotes. Os autores implementaram três estudos de caso distintos, cada um focado em um padrão específico, utilizando tecnologias como Node.js, Python, MongoDB e Docker. Os resultados demonstram que o padrão API Gateway é ideal para cenários de carga balanceada e oferece boa flexibilidade para gerenciar solicitações de múltiplos canais. O padrão Cadeia de Responsabilidade mostrou uma economia de cerca de 30% no uso de hardware comparado a uma implementação monolítica equivalente (megaservice). Já o padrão de Mensageria Assíncrona, implementado com RabbitMQ, mostrou-se eficaz para minimizar perdas de pacotes e melhorar a eficiência energética ao evitar a utilização de CPU em 100%, mantendo-a em níveis mais sustentáveis (~50%). O artigo conclui que a escolha do padrão deve ser baseada no cenário específico da aplicação, e que testes de carga e monitoramento contínuo são essenciais para o sucesso de uma arquitetura de microservices.

## 2. Fichamento Bibliográfico

*  _Percentil 95 (95th percentile)_: Métrica estatística mais significativa que a média para Acordos de Nível de Serviço (SLAs), pois representa um limite superior estatístico onde apenas 5% das amostras de tempo de resposta estão acima desse valor (página 2).
*  _Eficiência de Hardware (Hardware Efficiency)_: Métrica calculada para avaliar o quão eficientemente a arquitetura utiliza os recursos de hardware conforme o número de threads ou usuários aumenta. É derivada do tempo de resposta médio ou do percentil 95 (página 3, Equações 1 e 2).
*  _Padrão Chain of Responsibility (Cadeia de Responsabilidade)_: Padrão de design onde uma requisição é processada por uma cadeia de subserviços sequenciais, onde a saída de um se torna a entrada do próximo. Ideal para funções que processam dados compartilhados consecutivamente (página 4).
*  _Megaservice (Megaserviço)_: Considerado um antipadrão, é um serviço monolítico que agrupa muitas funcionalidades. Sua escalabilidade é ineficiente, pois escala todas as funcionalidades mesmo as que não necessitam, ao contrário dos microservices que escalam individualmente (página 5).
*  _Mensageria Assíncrona (Asynchronous Messaging)_: Padrão de comunicação preferido para grandes volumes de dados onde uma resposta imediata não é necessária. Utiliza filas (ex: RabbitMQ) para desacoplar serviços e gerenciar processos com tempos de serviço disparatos, melhorando a resiliência e eficiência energética (página 5).

## 3. Fichamento de Citações

*  _"The 95th percentile gives us an idea of the tail of the response time distribution. The further away it is from the mean, the longer the tail is."_
*  _"The ideal microservice design pattern for functions that process consecutively shared data is the chain of responsibility design pattern."_
*  _"In Case Study 2, we observed that this architecture allows us to scale back-end services independently, with a gain on the hardware usage of around 30% compared to the megaservice equivalent structure."_
*  _"Operating at 100% utilization causes an unwanted energy consumption."_
*  _"In the graph on the right, we see that the CPU settles down to around 50%."_
*  _"However, the needs of the organization should be taken into consideration while choosing a microservice architecture. In general, there is no single microservice pattern that is better than the others. Rather, each design pattern performs better in different scenarios."_