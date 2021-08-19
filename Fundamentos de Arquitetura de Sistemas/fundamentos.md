serviços web são API's que se comunicam por meio de redes sobre o protocolo HTTP, mas nem toda API é um serviço web.

## *Vantagens de usar um web service:*										

1. ·     Linguagem comum																	
2. ·     Integração
3. ·     reutilização de implementação
4. ·     segurança
5. ·     custos



## *principais tecnologias:*

## **mais usadas:**

1. ·     soap

2. ·     rest

   ## **linguagens de marcação:**

   1. ·     xml      < > 
   2. ·     json     { “ ” }





## *SOAP*

1. ·     Soap: Simple Object Access Protocol(protocolo simples de acesso ao objeto);
2. ·     Protocolo em XML para acesso em HTTP;
3. ·     É a definição de como os serviços web se comunicam;
4. ·     Faz integração entre aplicações , com todas as linguagens ;
5. ·     Usa o XML como linguagem padrão ;
6. ·     Pode ser usado por outros protocolos além do HTTP.





## *XML*

1. ·     Pode ser usado sem SOAP;
2. ·     Sem limites de tags;
3. ·     Criada na década de 90 pela W3C.

![image-20210818223819207](C:\Users\Ricardo\AppData\Roaming\Typora\typora-user-images\image-20210818223819207.png)

![im](C:\Users\Ricardo\Desktop/soap1.jpg)

1. ·     **SOAP Envelope:** possui toda a mensagem;

2. ·     **SOAP Header:** possui as informações dos atributos;

3. ·     **SOAP Body:** contém os detalhes da mensagem.                        

   ​                                   

   

WSDL: web services description language (funciona como um contrato de serviço em XML).

XSD: xml schema definiton (usado para definir a estrutura de dados que será validada no XML).





## *REST: Representational State Transfer:*

1. ·     Define a implementação de um serviço web;
2. ·     Faz a integração entre aplicações , clientes ;
3. ·     Aceita os formatos XLM, JSON, entre outros.

![image-20210818224524352](C:\Users\Ricardo\AppData\Roaming\Typora\typora-user-images\image-20210818224524352.png)





## *API: Application Programming Interface:*

São conjuntos de rotinas documentados e disponibilizados por uma aplicação para que outras aplicações possam consumir;

Principais métodos HTTP: 

1. ·   GET(chama);
2. ·   POST(cria);
3. ·   DELETE(exclui);
4. ·   PUT(atualiza).





## *JSON: JavaScript Object Notation*

1. ·     Formatação leve, usada para troca de mensagens entre sistemas;
2. ·     Utiliza chave, valor e listas ordenadas;
3. ·     Um dos formatos mais utilizados.

![image-20210818224642646](C:\Users\Ricardo\AppData\Roaming\Typora\typora-user-images\image-20210818224642646.png)





## *Códigos de Estado:*

1. ·     1xx informativo;
2. ·     2xx sucesso;
3. ·     3xx redirecionamento;
4. ·     4xx erro do cliente;
5. ·     5xx erro do servidor.



## 																	

## 																	Monolito(apenas 1 serviço)

![image-20210818224818912](C:\Users\Ricardo\AppData\Roaming\Typora\typora-user-images\image-20210818224818912.png)

## *vantagens*

1. ·     Baixa complexidade;

2. ·     Monitoramento simplificado
   ​			Apenas 1 serviço.

## *desvantagens*

1. ·     Stack única

   ​			Sistema roda apenas em uma linguagem;

2. ·     Compartilhamento de recursos;

3. ·     Acoplamento;

4. Mais complexo a escalabilidade.





## 																							

![image-20210818225510162](C:\Users\Ricardo\AppData\Roaming\Typora\typora-user-images\image-20210818225510162.png)

| Microserviços #1              |                                                              |
| ----------------------------- | ------------------------------------------------------------ |
| vantagens                     | desvantagens                                                 |
| ·     Stack dinâmica          | ·     Acoplamento                                            |
| ·     Simples escalabilidade  | ·     Monitoramento mais complexo                            |
|                               | ·     Provisionamento mais complexo                          |
|                               |                                                              |
| Microserviços #2              |                                                              |
| vantagens                     | desvantagens                                                 |
| ·     Stack dinâmica          | ·     Monitoramento mais complexo                            |
| ·     Simples escalabilidade  | ·     Provisionamento mais complexo                          |
| ·     Desacoplamento.         |                                                              |
|                               |                                                              |
|                               |                                                              |
| Microserviços #3 (pipeline)   |                                                              |
| vantagens                     | desvantagens                                                 |
| ·     Stack dinâmica;         | ·     Provisionamento mais complexo;                         |
| ·     Simples escalabilidade; | ·     Plataforma inteira depende do gerenciador de pipeline. |
| ·     Desacoplamento;         |                                                              |
| ·     Menor complexidade.     |                                                              |

## 



## *Conceitos básicos de IOT:*

1. Things, Cloud, Intelligence.





## *Locais de implantação do IC*

1. ·     Smart Building(capacidade de coletar determinados dados e utilizar de forma inteligente);
2. ·     Smart Home(coleta de dados por sensores);
3. ·     Wearables(gerenciador de atividades);
4. ·     Agriculture(sensor que gerencia o modo de cultivo);
5. ·     Smart Transportation(comunicação entre veiculos);
6. ·     RFID Supply Chain(monitoramento do ciclo de um determinado produto);
7. ·     Energy Efficiency(coleta de dados de fontes geradoras e fontes consumidoras de energia).





## *Desafio da IC*

1. ·     Privacidade e Segurança;
2. ·     Total de dipositivos conectados na rede;
3. ·     Processar e armazenar diversas quantidade de informações;
4. ·     Gerar valor das informações coletadas.





## *Atributos a ser considerado na escolha*

1. ·     Baixo consumo de energia;
2. ·     Rede de dados ilimitado;
3. ·     Resiliência;
4. ·     Segurança;
5. ·     Customização;
6. ·     Baixo custo.



| *Arduíno*                      | Embarcados (MCUs)                           |
| ------------------------------ | ------------------------------------------- |
| Plataforma de prototipagem     | Uso industrial, médico, militar, transporte |
| Com entradas e saídas digitais | Microcontrolador de chip único              |
| Com entradas e saídas digitais | Sistema operacional real time               |
| Escrito em C/C++               | Embarcado                                   |
| Interface serial ou USB        |                                             |
| Shields.                       |                                             |
|                                |                                             |
|                                |                                             |





## *Protocolo MQTT(assíncrono)*

1. ·     Criado pela IBM para conectar sensores de pipelines de petróleo a satélite;
2. ·     Protocolo de mensagem assíncrona(M2M);
3. ·     Padrão OASIS suportado pelas linguagens de progrmação mais populares
4. ·     Base na pilha do TCP/IP





*Modelo cliente servidor:* é síncrono(toda vez que o client faz request, ele aguarda a resposta para retornar o serviço. Ex: client digita o endereço da internet e o servidor devolve para o client

*Modelo Publish/Subscribe:* fornecedor(envia a mensagem) e consumidor (inscrito recebe a mensagem)





## *A flexibilidade dos Tópicos*

Protocolo - Broker - User Identifier - Sensor - Information Type





![image-20210818231415708](C:\Users\Ricardo\AppData\Roaming\Typora\typora-user-images\image-20210818231415708.png)

## *QoS (0)*

Nível mínimo(0) de menor esforço(menor custo), sem garantia de entrega, a mensagem não é retransmitida;   

## *Nível(1)* 

Garante a entrega da mensagem no mínimo uma vez ao recebedor, a mensagem pode ser retransmitida se não houver confirmação; 

## *Nível(2)* 

Garante a entrega da mensagem no mínimo uma vez ao recebedor, a mensagem pode ser retransmitida se não houver confirmação;





## *Cloud*

1. ·     Grande e cada vez maior número de devices conectados;
2. ·     TBs ou PBs de informações;
3. ·     Potencial de escala global.

