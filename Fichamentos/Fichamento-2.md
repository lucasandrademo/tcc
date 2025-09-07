# Event Driven Architecture: An Exploratory Study on The Gap between Academia and Industry

N. Trabelsi, C. Politowski and G. E. Boussaidi, "Event Driven Architecture: An Exploratory Study on The Gap between Academia and Industry," 2023 IEEE/ACM 5th International Workshop on Software Engineering Research and Practices for the IoT (SERP4IoT), Melbourne, Australia, 2023, pp. 25-32, doi: 10.1109/SERP4IoT59158.2023.00010.

## 1. Fichamento de Conteúdo

O artigo realiza um estudo exploratório sobre a arquitetura orientada a eventos (EDA), com foco na lacuna entre as definições acadêmicas e as implementações industriais, especialmente no contexto de aplicações de IoT. Os autores identificam que, embora a EDA seja amplamente reconhecida por promover desacoplamento e escalabilidade, não há um consenso na literatura sobre seus componentes e interações, nem uma padronização na forma como as plataformas industriais a implementam. O estudo seleciona e analisa três plataformas populares — Apache Kafka, AWS EventBridge e Google Eventarc — com base em elementos extraídos de oito estudos acadêmicos. Os resultados mostram que as plataformas implementam apenas um subconjunto dos elementos teóricos, variam na forma de especificação e categorização de eventos, e não suportam topologias mais complexas, como a de mediador. Conclui-se que há uma necessidade urgente de padronização e diretrizes claras para o projeto de EDAs, especialmente em cenários de IoT.

## 2. Fichamento Bibliográfico 

* _Evento_: Uma mudança no estado de um componente de software que é de interesse para outro sistema ou componente. Pode ser classificado por nível de abstração, complexidade, domínio ou notabilidade (página 2).
* _Produtor (Publisher)_: Componente que atua como provedor de eventos, podendo ser fonte ou publicador dos eventos (página 3).
* _Serviço de Notificação de Eventos (ENS)_: Componente responsável por gerenciar assinaturas e disseminar notificações de eventos entre produtores e consumidores (página 3).
* _Topologias de EDA_: Broker (roteamento simples) e Mediator (lógica de processamento centralizada para transformar eventos iniciais em sequências de eventos processados) (página 4).

## 3. Fichamento de Citações

* _"An event is a change in the state of a software component which is of interest to another system or component."_
* _"EDA is an architectural pattern where components communicate by reacting to events published by other components. This enables high decoupling between software components."_
* _"None of the platforms offers functions to translate a published event to a sequence of calls to applications or services and/or transmission of events to consumers, they do not natively support the mediator topology."_
* _"This lack of a commonly accepted specification for defining the attributes of exchanged events might limit the interoperability of EDA solutions developed based on the platforms currently offered by the industry."_