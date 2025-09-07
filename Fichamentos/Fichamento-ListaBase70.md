# Measuring the Benefits of CI/CD Practices for Database Application Development 

J. Fluri, F. Fornari and E. Pustulka, "Measuring the Benefits of CI/CD Practices for Database Application Development," 2023 IEEE/ACM International Conference on Software and System Processes (ICSSP), Melbourne, Australia, 2023, pp. 46-57, doi: 10.1109/ICSSP59042.2023.00015.

## 1. Fichamento de Conteúdo

O artigo investiga os benefícios da adoção de práticas de Integração Contínua e Entrega Contínua (CI/CD) no desenvolvimento de aplicações de banco de dados, uma área onde a automação ainda é incipiente e os processos manuais predominam. Os autores propõem e implementam um pipeline de CI/CD adaptado para contextos de banco de dados, incorporando etapas como análise estática de código, migração automatizada de esquemas, testes unitários e de sistema, e mecanismos de rollback. O estudo é baseado em dois casos industriais reais: um data warehouse em uma seguradora suíça (UC1-DWH) e um back-end de banco de dados em uma administração pública europeia (UC2-BE). Por meio de uma abordagem mista — com medições quantitativas (como número de falhas em deploy, lead time e frequência de implantações) e entrevistas qualitativas com desenvolvedores —, os autores demonstram que a automação do pipeline resulta em redução significativa de falhas, maior frequência de implantações, maior estabilidade e redução da carga cognitiva da equipe. No entanto, limitações organizacionais — como janelas fixas de release — impediram a redução do lead time. O artigo oferece um blueprint de pipeline e infraestrutura de CI/CD para bancos de dados e discute desafios, trade-offs e direções futuras para pesquisa e prática.

## 2. Fichamento Bibliográfico 

* _Integração Contínua e Entrega Contínua (CI/CD)_ refere-se a práticas de automação no desenvolvimento de software que visam integrar, testar e entregar código de forma frequente e confiável, reduzindo trabalho manual e acelerando o tempo de entrega (página 1).
* _Database Schema Evolution_ é o processo de evolução do esquema de um banco de dados ao longo do tempo, que inclui mudanças na estrutura de tabelas, views, procedures e outros objetos, e é um dos principais desafios para a automação em CI/CD (página 2).
* _Princípio do Least Privilege_ é uma prática de segurança que determina que usuários e sistemas devem ter apenas as permissões mínimas necessárias para realizar suas funções, aplicado também a pipelines de CI/CD para limitar acesso a repositórios e ambientes (página 9).
* _Cognitive Load_ (carga cognitiva) refere-se ao esforço mental exigido dos desenvolvedores para realizar tarefas manuais repetitivas, como integração e deploy, que pode ser reduzido com automação (página 9).
* _Trunk-Based Development_ é uma estratégia de desenvolvimento onde todos os desenvolvedores trabalham em um único branch principal (trunk), evitando long-lived feature branches e facilitando a integração contínua (página 10).

## 3. Fichamento de Citações 

* _"Automation reduces the time it takes from defining software requirements to deploying the software in production."_
* _"Database schema changes are considered a technical challenge when adopting CD."_
* _"The measurements reveal that the number of deployments increased with the automated CI pipeline and the number of failed deployments decreased, making deployments more reliable."_
* _"The mental load of the development teams was reduced by eliminating manual tasks required before pipeline automation."_
* _"Fixed-release windows prevented changes from going through the pipeline outside those set release times, requiring the developers to keep track of the deployment of their changes."_
* _"The biggest problem perceived by the developers now are the fixed-release windows that do not allow them to promote changes into production when features are done."_