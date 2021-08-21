Arquitetura em mensageria

| Vantagem                                                     | Desvantagem                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Desacoplamento(não possui comunicação entre si)              | Single point of failure(com apenas 1 falha o sistema inteiro quebra) |
| Fácil plug & play(facilidade em aceitar novos serviços)      | Difícil monitoramento(sendo assíncrona não é possível fazer o monitoramento) |
| Comunicação assíncrona(o serviço continua sem precisar esperar a resposta) |                                                              |
| Simples escalabilidade(gerencia e distribui de uma forma melhor a escala de serviços) |                                                              |
| broadcasting(comunicação forte entre os serviços)            |                                                              |
| Permite Event Source(diversos serviços sendo produzidos)     |                                                              |



Gerenciamento de Erros

1. Dead letter queue(identifica o erro da mensagem e guarda em uma fila de re-tentantivas)
2. Monitoramento entre serviços
3. Rastreamento de fluxo



Business Inteligence (BI) é composto por:

1. Feramentas
2. Infraestrutura
3. Profissionais
4. Dados
   1. operacionais
   2. gerenciais
   3. pesquisa de campo
   4. indicadores de mercado

Solution

1. Infraestrutura

2. Gerenciamento dos dados

3. Analytics

4. Compartilhamento

5. Ferramentas gerais

   ​		

   

   ​															OLTP														OLAP

|                              | On-Line Transaction Processing(muitos usuários)              | On-Line Analytical Processing(poucos usuários)       |
| ---------------------------- | ------------------------------------------------------------ | ---------------------------------------------------- |
| foco                         | análise empresarial e tomada de decisão                      | execução operacional do negócio                      |
| performance                  | leitura e geração de análises e relatórios                   | alta velocidade na manipulação de dados operacionais |
| estrutura de dados           | modelagem dimensional                                        | modelo relacional normalizado                        |
| armazenamento                | em Data Warehouse                                            | em sistemas convencionais de BD                      |
| abrangência                  | é útil aos gestores e analistas nas decisões                 | útil aos técnicos e analistas e vários usuários      |
| frequência de atualização    | baixa(no processo de carga dos dados, sendo diária semanal, mensal ou anual) | alta(no momento da transação)                        |
| volatilidade                 | dados históricos e não voláteis                              | dados voláteis,  passíveis de modificação e exclusão |
| tipos de permissões de dados | apenas inserção e leitura, para usuário apenas leitura       | leitura, inserção, modificação e exclusão de dados   |

![oltp e olap](C:\Users\Ricardo\Desktop\oltp e olap.jpg)



Big Data or Data Lake(grande volume de dados)

| Dados Estruturados                                | Dados Semi-Estruturados                                      | Dados Não Estruturados                                       |
| ------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| segue uma ordem específica para manusear os dados | segue uma estrutura básica não exigindo um padrão(xml, json) | contém várias informações de dados estruturados e semi-estruturados |
|                                                   | NoSQL                                                        |                                                              |
|                                                   | alguns NoSQL(mongo, cassandra, apache)                       | hadoop, spark, storm, ceph, datatorrent, bigquery            |



Cloud Computing

1. Gerenciamento de hardware / software
2. Provedores de servidor e armazenamento
3. Pague o que consumir
4. Iaas(Infrastructure as a service) / Paas(Plataform as a Service)/ Baas(Backend as a service)



Disponibilidade

1. Iaas: sem se preocupar com  hardware e internet
2. Paas: auto scale on the go(disponibilidade de mais máquinas para suprir o aumento de acessos)
3. Baas: facilidade no desenvolvimento de Front end, por não ser preciso desenvolver o Back end
4. Kubernets(K8S)
5. Múltiplos nodos(para alta demanda)
6. Load balancer(gerenciamento para melhor distribuição de serviços)



Servless

1. Sem servidor
2. Sem serrviço "rodando"
3. Sem down time



DevOps

​	É definido como um conjunto de práticas que integram e automatizam os processos entre as equipes de desenvolvimento, operações e de apoio a produção rápida e confiável de software

Framework CALMS

1. Culture: União e disposição no desenvolvimento e operações(resolução de problemas humanos);
2. Automation: sem trabalho manual repetitivo, e sim a produção de processos repetitivos, sendo mais produtivo;
3. Learn: Ser objetivos, enxutos e otimizar o fluxo;
4. Measurement: cíclico e infinito;
5. Sharing: O compartilhamento de informações torna o time autossustentável e evita que os processos se tornem dependentes.

Os trê caminhos

1. Flow: Otimização do fluxo entre a demanda e a entrega, <u>a chave deste caminho é a aplicação de metodologias ágeis e a automatização dos processos</u>; 

   ​					Dev(Business)  -------------->    Ops(Customer)

2. Feedback: Ciclos rápidos que visam resolver problemas o quanto antes, <u>a chave é o monitoramento</u>; 

   ​					Dev(Business)  -------------->    Ops(Customer) --------------> Dev(Business)

3. Learning: o aprendizado contínuo visa gerar conhecimento através da experimentação. Este caminho produz segurança psicológica, a chave é o trabalho dinâmico, com times;

   ​					Dev(Business)  -------------->    Ops(Customer) --------------> Dev(Business) (loop)

Entregando Software

​	plan -----> code -----> build -----> test -----> release -----> deploy -----> operate -----> monitor


