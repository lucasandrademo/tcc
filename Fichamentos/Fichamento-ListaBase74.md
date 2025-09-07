# Modular Monolith: Is This the Trend in Software Architecture?

Ruoyu Su and Xiaozhou Li. 2024. Modular Monolith: Is This the Trend in Software Architecture? In Proceedings of the 1st International Workshop on New Trends in Software Architecture (SATrends '24). Association for Computing Machinery, New York, NY, USA, 10–13. https://doi.org/10.1145/3643657.3643911

## 1. Fichamento de Conteúdo

O artigo investiga a arquitetura de software conhecida como "Modular Monolith", que tem ganhado atenção recentemente, especialmente após o lançamento do framework "Service Weaver" pelo Google, que permite escrever aplicações como monólitos modulares e implantá-las como microsserviços. Os autores realizam uma revisão sistemática de literatura cinzenta para compreender a definição, os frameworks e os casos de uso dessa arquitetura. Os resultados mostram que o Modular Monolith combina vantagens dos monólitos tradicionais (como simplicidade de desenvolvimento e implantação) e dos microsserviços (como modularidade e escalabilidade). Foram identificados três frameworks principais (Service Weaver, Spring Modulith e Light-hybrid-4j) e quatro casos de uso em empresas como Shopify, Appsmith, Gusto e PlayTech. Conclui-se que o Modular Monolith é uma alternativa viável aos microsserviços e pode servir como um passo intermediário em migrações futuras. O estudo oferece insights valiosos para pesquisadores e profissionais na escolha de arquiteturas de software.

## 2. Fichamento Bibliográfico 

* _Modular Monolith_ é um padrão de arquitetura de software que combina a simplicidade de um monólito com a modularidade dos microsserviços, organizando o sistema em módulos fracamente acoplados com dependências bem definidas (página 2).
* _Service Weaver_ é um framework de código aberto desenvolvido pelo Google que permite escrever aplicações como um monólito modular em Go e implantá-las como um conjunto de microsserviços, separando o código do modelo de implantação (página 3).
* _Spring Modulith_ é um projeto experimental do Spring que facilita a construção de aplicações modulares monólitas no ecossistema Spring, fornecendo convenções e APIs para declarar e validar módulos lógicos (página 3).
* _Light-hybrid-4j_ é um framework construído sobre a plataforma Light-4j para arquiteturas modulares monólitas e serverless, oferecendo flexibilidade de implantação e redução de custos (página 4).
* _Microservices_ são uma abordagem arquitetural onde a aplicação é decomposta em serviços independentes, implantados e escalados separadamente, mas que podem introduzir complexidade e custos adicionais (página 1).

## 3. Fichamento de Citações 

* _"Modular Monolith is a software architecture pattern that strategically combines the simplicity of a monolithic structure with the advantages of microservices."_
* _"Service Weaver provides the idea of decoupling the code from how code is deployed."_
* _"Shopify is a great example that has used this approach as an alternative to microservice decomposition."_
* _"The goal is to achieve independence and isolation for each module, allowing them to be worked on independently while still being deployed collectively as a single unit."_
* _"Modular monolith is an alternative way to microservices, and it also could be a previous step before systems migrate to microservices."_
* _"Google found that the expense of maintaining multiple different microservice binaries with separate configuration files, network endpoints, and serializable data formats significantly slowed down the development of microservice-based applications."_