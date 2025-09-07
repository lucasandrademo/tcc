# Back to the Future: From Microservice to Monolith

Su, Ruoyu & Li, Xiaozhou & Taibi, Davide. (2023). Back to the Future: From Microservice to Monolith. 10.48550/arXiv.2308.15281. 

## 1. Fichamento de Conteúdo

O artigo investiga um fenômeno recente na indústria de software: a migração de sistemas baseados em arquitetura de microservices de volta para uma arquitetura monolítica. Os autores realizam uma revisão multivocal da literatura (incluindo literatura acadêmica e cinzenta) para entender as razões por trás dessa reversão, os aspectos-chave a serem considerados durante o processo e as opiniões de profissionais do setor. Foram identificados quatro casos concretos de empresas que realizaram essa migração reversa: Istio, Amazon Prime Video, Segment e InVision. As cinco principais razões para a reversão são: custo, complexidade, escalabilidade, desempenho e organização. O estudo também sintetiza seis aspectos críticos a serem observados durante a transição, como parar de desenvolver novos serviços, consolidar caminhos e testá-los, e unificar o armazenamento de dados. As opiniões dos profissionais são divididas, mas a maioria concorda que a decisão deve ser baseada em uma avaliação cuidadosa do contexto específico do sistema e da organização, e não seguir tendências cegamente.

## 2. Fichamento Bibliográfico 

* _Custo_: Razão mais comum para a reversão. A arquitetura de microservices, especialmente com componentes serverless, pode gerar custos operacionais e de infraestrutura significativamente mais altos do que uma abordagem monolítica, como evidenciado pela redução de 90% nos custos da Amazon Prime Video (página 3).
* _Complexidade_: A natureza distribuída dos microservices introduz complexidade no gerenciamento de múltiplos repositórios, bibliotecas compartilhadas divergentes e na coordenação entre diferentes equipes e tecnologias, tornando o sistema difícil de manter e evoluir (página 3).
* _Escalabilidade_: Em certos cenários, a escalabilidade independente dos microservices pode se tornar uma desvantagem, criando gargalos inesperados (como no caso da AWS Step Functions na Prime Video) e uma sobrecarga operacional significativa para gerenciar e dimensionar cada serviço individualmente (página 3).
* _Princípio do barramento de mensagens (Message Bus)_: Estratégia chave durante a transição para garantir comunicação contínua entre os componentes que estão sendo consolidados, permitindo uma migração gradual e sem interrupções, usando ferramentas como Apache Kafka (página 4).
* _Design modular_: Princípio fundamental a ser mantido mesmo após a migração para um monolito. Organizar o código em módulos distintos com limites bem definidos ajuda a manter a separação de concerns e a facilidade de manutenção, oferecendo alguns dos benefícios de microservices com a simplicidade de um monolito (página 4).

## 3. Fichamento de Citações

* _"Microservices Also Have a Dollars-And-Cents Cost"_
* _"moving the service from microservice back to a monolith reduced the infrastructure cost by over 90%"_
* _"The microservice architecture causes head-of-line blocking, causes delays in all destinations"_
* _"the benefits of Conway's Law became a burden on the legacy team because of this unsuitable 'size'"_
* _"Microservices are dead, long live the monolith"_
* _"the recommendation for architecture depends on the type of project"_