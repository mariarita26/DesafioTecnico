# Desafio Técnico – Estágio em Desenvolvimento SQL

## Considere um contexto bem próximo da nossa realidade, onde precisamos construir uma base de dados para controlar as faturas de clientes de um varejista, bem como os pagamentos realizados, realizar consultas e implementar pequenas rotinas. Vamos lá…

### 1. Criar os scripts para a estrutura de banco, conforme indicações abaixo (aqui utilize SQL ANSI):

● Cliente [idcliente, nome, idade, statusbloqueio, limitecredito];

● Fatura [idfatura, datavencimento, valor, status];

● Pagamento [idpagamento, datapagamento, valor];

  a. Popular as tabelas com no máximo 10 registros cada;
  
  b. Criar suas respectivas chaves primárias e estrangeiras;
  
  c. Disponibilizar o modelo entidade-relacionamento resultante.
  
  
### 2. Desenvolver os scripts para as seguintes consultas (aqui utilize SQL ANSI):

a. Consultar clientes com idade entre 18 e 21 anos que possuem limite de crédito maior ou igual a 1.000 reais.
  Retorno: Total de clientes.
  
b. Consultar clientes cujo pagamento foi realizado no dia do vencimento da fatura.
  Retorno: Data de vencimento e a quantidade.
c. Consultar clientes que realizaram o pagamento 1 dia antes da data de vencimento da fatura.
  Retorno: Id do cliente, valor da fatura e data de pagamento,
d. Consultar clientes com pagamento da fatura em atraso.
  Retorno: Id do cliente, nome, valor da fatura, data de vencimento, status (P=Pago, A=Atraso), e quantidade de dias em atraso.
e. Consultar cliente bloqueado por atraso no pagamento da fatura. (clientes com mais de 3 dias de atraso devem ser bloqueados)
  Retorno: Id do cliente, nome, status de bloqueio (A=Ativo, B=Bloqueado), id da fatura, valor da fatura e a quantidade de dias em atraso.


### 3. Implementar bloco anônimo com as seguintes instruções e utilizando estruturas de repetição (laços), sempre que possível (aqui utilize PL/SQL):

a. Bloco anônimo 1: Inserir pagamento e atualizar status da fatura.

b. Bloco anônimo 2: Atualizar o limite de crédito para 0, de todos os clientes que estão bloqueados por atraso no pagamento da fatura.

c. Bloco anônimo 3: Implementar rotina para exclusão de todos os clientes que não possuem nenhuma fatura.



## Modelo Conceitual

![Conceitual](https://user-images.githubusercontent.com/89050107/219829332-01ee8072-3b28-4c29-b67d-66d3f622fa71.png)

## Modelo Lógico

![lógico](https://user-images.githubusercontent.com/89050107/219923077-a356bb49-ce06-4009-b38b-92302abe7517.jpg)

