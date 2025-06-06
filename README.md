# SQL-Join-Vendas-Clientes
Projeto simples em SQL usando JOIN para consultar nome dos clientes e total de vendas. Feito para praticar os conceitos básicos que estou aprendendo.
# Projeto de SQL com JOIN - Clientes e Vendas

Esse projeto eu fiz pra treinar o que eu aprendi até agora de SQL, principalmente o JOIN.

Ainda estou aprendendo, mas consegui juntar duas tabelas e fazer uma consulta que mostra o nome dos clientes junto com o valor da venda.

---

## O que eu usei aqui:

- SELECT
- FROM
- JOIN
- ON

## Tabelas usadas:

### Tabela: clientes

| id  | nome   | cidade            |
|-----|--------|------------------|
| 201 | Ana    | São Paulo        |
| 202 | Carlos | Belo Horizonte   |
| 203 | Júlia  | Recife           |

### Tabela: vendas

| id  | id_cliente | total_vendas |
|-----|-----------|--------------|
| 1   | 201        | 150           |
| 2   | 202        | 300          |
| 3   | 203        | 120          |
| 4   | 201        | 250          |

---

## Consulta que eu usei:

'SQL'
SELECT clientes.nome, vendas.total_vendas
FROM clientes
JOIN vendas
ON vendas.id_cliente = clientes.id


Essa consulta me mostrou o nome do cliente e quanto ele gastou em cada venda. A ligação entre as tabelas foi feita pelo id do cliente.

- Resultado -

  nome      total_vendas
  Ana       150
  Carlos    300
  Júlia     120
  Ana       250
