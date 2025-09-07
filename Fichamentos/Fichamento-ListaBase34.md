# One Size Does Not Fit All: An Empirical Study of Containerized Continuous Deployment

Yang Zhang, Bogdan Vasilescu, Huaimin Wang, and Vladimir Filkov. 2018. One size does not fit all: an empirical study of containerized continuous deployment workflows. In Proceedings of the 2018 26th ACM Joint Meeting on European Software Engineering Conference and Symposium on the Foundations of Software Engineering (ESEC/FSE 2018). Association for Computing Machinery, New York, NY, USA, 295–306. https://doi.org/10.1145/3236024.3236033

## 1. Fichamento de Conteúdo

O artigo realiza um estudo empírico sobre fluxos de trabalho de implantação contínua (CD) utilizando contêineres Docker, com foco em projetos de código aberto hospedados no GitHub e registrados no Docker Hub. Os autores identificam dois workflows predominantes: o baseado em builds automáticos do Docker Hub (DHW) e o baseado em ferramentas de integração contínua, como Travis CI e CircleCI (CIW). Por meio de uma abordagem mista, combinando survey qualitativo com 168 desenvolvedores e análise quantitativa de 855 projetos e mais de 133 mil builds, o estudo explora as motivações, barreiras e trade-offs associados a cada abordagem. Os resultados mostram que, embora ambos os workflows apresentem vantagens e desvantagens, a escolha entre eles deve considerar fatores como experiência da equipe, necessidade de controle versus simplicidade, latência de build e estabilidade de configuração. O artigo conclui que não existe uma solução única para todos os casos, destacando a importância de decisões informadas baseadas em evidências empíricas.

## 2. Fichamento Bibliográfico 

* _Continuous Deployment (CD)_ é uma prática de engenharia de software que visa automatizar a entrega e implantação de software após quaisquer alterações no código, permitindo que o software esteja sempre em estado implantável (página 1).
* _Docker Hub Auto-Builds (DHW)_ é um workflow no qual o Docker Hub constrói automaticamente imagens a partir de arquivos fonte no GitHub sempre que ocorrem mudanças, utilizando webhooks para acionar os builds (página 2).
* _CI-Based Workflow (CIW)_ é um workflow no quais ferramentas de CI como Travis CI ou CircleCI são utilizadas para construir e publicar imagens Docker durante o estágio de build e teste, com posterior push para o Docker Hub (página 2).
* _Build latency_ refere-se ao tempo decorrido desde o início até o fim de um build bem-sucedido, sendo uma métrica crítica para avaliar a eficiência do processo de CD (página 7).
* _Dockerfile stability_ é medida pelo número de alterações no arquivo Dockerfile em janelas de tempo, indicando a maturidade e a consistência da configuração do contêiner ao longo do tempo (página 8).


## 3. Fichamento de Citações

* _"Continuous deployment (CD), also referred to as continuous delivery, is the fast-paced, automation-heavy software engineering approach in which teams work in short iterations to produce software that is deployable (production ready) at any time."_
* _"Containerization has transformed CD workflows, promising additional speedups and higher level of abstraction."_
* _"We found that two Docker image deployment workflows were most prominent: (1) a Docker Hub auto-builds Workflow (denoted DHW), where the registry itself builds the image automatically whenever GitHub source files change; and (2) a CI-based Workflow (denoted CIW), where CI tools build images during the build and test stage, then publish to Docker Hub."_
* _"Our findings indicate that developers face trade-offs when choosing between different CD workflows with respect to configurability, simplicity, requirements, performance, stability, developer experience, etc."_
* _"Release frequency tends to decrease over time. But DHW tends to have lower release frequency than CIW."_
* _"Build latency tends to increase slightly over time. Interestingly, DHW tends to have longer build latency than CIW."_