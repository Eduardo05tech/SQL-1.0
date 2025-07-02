# SQL-1.0

Considere as seguintes tabelas:
Tabela 'clientes':
| id_cliente | nome |
|------------|------------|
| 1 | João Silva |
| 2 | Ana Lima |
| 3 | Carlos Luz |
Tabela 'pedidos':
| id_pedido | id_cliente | data_pedido |
|-----------|------------|-------------|
| 101 | 1 | 2023-10-15 |
| 102 | 2 | 2023-10-20 |
| 103 | 1 | 2023-11-01 |

Escreva uma query que retorne o nome do cliente e a data de cada pedido realizado.

SELECT clientes.nome, pedidos.data_pedido
FROM clientes
JOIN pedidos ON clientes.id_cliente=pedidos.id_cliente;
