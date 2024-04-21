# Segmentação de Clientes


## Contexto do Problema

Este projeto visa segmentar os clientes de uma loja de e-commerce por meio da análise RFM (Recency, Frequency, Monetary) para proporcionar marketing personalizado, como e-mails com informações relevantes para cada cliente. Utilizando essa abordagem, buscamos customizar o marketing, considerando a última interação do cliente, a frequência de compras e o valor total gasto. Ao categorizar os clientes, como "VIPs" ou "em risco de churn", podemos desenvolver estratégias de marketing mais direcionadas e eficazes, com o objetivo de fortalecer o relacionamento com o cliente e otimizar o valor para o negócio.


## Descrição dos Dados

Vamos trabalhar com os dados da Ulist, que esta disponivel na plataforma Kaggle.

As variaveis que vamos trabalhar nesse projeto são:


Attribute | Definition
------------ | -------------
|amostra | vai ser uma numeração crescente dos dados.ex: 1, 2, 3, 4, 5 ...  |     
|id_cliente | número usado pelo cliente na compra |             
|id_unico_cliente | número único dado para cada cliente em função do ip dele, independente da compra |       
|item_id | número de identificação do item comprado |              
|cep_cliente | CEP de moradia ou de entrega do cliente |              
|cidade_cliente | vai ser a cidade de onde foi feito o pedido |          
|estado_cliente | Estado de onde foi feito o pedido |         
|id_pedido | número de identificação da compra |               
|status_pedido | status de entrega ou não do pedido |             
|horario_pedido |  horário e data em que o pedido foi feito |           
|pedido_aprovado | horário e data em que o entregador recebeu o pedido |          
|pedido_entregador | ... |       
|pedido_entregue | data e horário em que o pedido foi entregue |         
|data_estimada |  horário e a data estimada de entrega |            
|id_vendedor | número de identificação do vendedor |               
|preco | preço do produto |                    
|frete | preço do frete |                  
|pagamento_sequencial | caso o cliente faça uma compra utilizando mais de um método de pagamento ele aciona um pagamento sequencial, que vai ser criado para acomodar todas as ordens de pagamento |    
|pagamento_tipo | método de pagamento, se foi boleto, cartão de crédito, cartão de débito |           
|pagamento_prestacoes | número de prestações escolhido pelo cliente |     
|pagamento_valor | o valor pago |          
|review | review de todo o processo |                  
|categoria | categoria do item comprado |                
|categoria_ingles | nome da categoria em inglês |        
|cep_vendedor | CEP do vendedor |             
|cidade_vendedor | cidade do vendedor |        
|estado_vendedor |  Estado do vendedor |    



## Resultados e Insights

Neste projeto, empregamos um dos métodos mais utilizados de clusterização, o K-means, para segmentar nossos clientes com base em seu comportamento RFM. Determinamos que o número ideal de clusters para cada conjunto RFM era 4, resultando na criação de uma nova variável denominada Pontuação. Essa pontuação foi fundamental para classificar os clientes em diferentes segmentos, nomeadamente Master, Business, Inativo e Premium. A seguir, apresentamos a distribuição dos clientes dentro desses segmentos.


<div align=center>

![H1](Imagens/img.png 'sadas')
</div>



### Ações a serem tomadas

- Recuperar os Inativos (promoções e cupons especiais);

- Fornecer descontos especiais de frete aos Master;

- Descontos especiais aos Premium e atendimento especializado.



#### Frequência X Recência:

<div align=center>

![H1](Imagens/img1.png 'sadas')
</div>


#### Receita X Frequência:

<div align=center>

![H1](Imagens/img2.png 'sadas')
</div>


#### Receita X Recência:

<div align=center>

![H1](Imagens/img3.png 'sadas')
</div>




