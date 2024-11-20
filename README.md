# Projeto Conceitual de Banco de Dados - e-commerce

## Descrição
Este projeto foi desenvolvido como parte da Bootcamp Suzano - Análise de Dados com Power BI, promovida pela Digital Innovation One (DIO). O objetivo principal foi a criação de uma modelagem conceitual de um banco de dados voltado para o setor de e-commerce, utilizando o MySQL Workbench como ferramenta de design e estruturação.
O banco de dados foi planejado para atender às necessidades de gestão de pedidos, entregas, clientes (Pessoa Física e Jurídica), controle de estoque, produtos e fornecedores.

## Principais Entidades e Relacionamentos
`1. Produto`
- Os produtos são vendidos por uma única plataforma online, mas podem ser fornecidos por diferentes vendedores (terceiros).
-  Cada produto possui um fornecedor.
-  Um pedido pode conter um ou mais produtos.

`2. Cliente`
- Os clientes podem se cadastrar na plataforma com CPF (Pessoa Física) ou CNPJ (Pessoa Jurídica).
- Uma conta pode ser associada a Pessoa Física ou Pessoa Jurídica, mas nunca ambas simultaneamente.
- O endereço do cliente irá determinar o valor do frete.
- Um cliente pode comprar mais de um pedido, e cada pedido possui um período de carência para devolução dos produtos.

`3. Pedido`
- Os pedidos são criados pelos clientes e armazenam informações da compra, endereço e status da entrega.
- Cada pedido pode conter um ou mais produtos.
- Os pedidos podem ser cancelados antes da entrega.

`4. Fornecedor & Estoque`
- Cada produto está vinculado a um fornecedor que garante a sua disponibilidade.
- O estoque é gerenciado para monitorar a quantidade de produtos disponíveis na plataforma.

`5.Pagamento`
- O cliente pode cadastrar várias formas de pagamento e utilizar uma delas.

`6.Entrega`
- As entregas possuem um status de acompanhamento além do código de rastreio.
  
