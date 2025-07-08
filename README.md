# 📊 Dashboard de Logística – Estoque

Este projeto é um dashboard interativo desenvolvido no **Power BI**, com o objetivo de realizar a **análise de estoque e logística** de uma empresa. Os dados são provenientes de um **banco de dados SQL Server**, simulando um cenário real de integração entre banco de dados e visualização de indicadores.

---

## 🗂️ Fonte de Dados

Os dados utilizados foram extraídos de um banco de dados SQL Server, contendo as seguintes tabelas principais:

- `Produtos`: Nome, categoria, estoque mínimo e valor unitário.
- `Entradas`: Informações das entradas no estoque (data, produto, fornecedor e quantidade).
- `Saídas`: Informações de saída dos produtos (data, produto, destino e quantidade).
- `Estoque`: Estoque atual por produto.
- `Fornecedores`: Origem dos produtos (Fábrica, Atacadista, Distribuidor) e cidade.
- `Calendário`: Tabela de datas para suporte às análises temporais.

---

## 📈 Métricas e Medidas (DAX)

As principais medidas criadas com DAX:

- `Estoque Total Atual`: Soma da coluna `EstoqueAtual`.
- `Valor em Estoque`: Soma de (`EstoqueAtual` × `ValorUnitario`).
- `Qtd Produtos`: Distinct count dos produtos cadastrados.
- `Produtos com Estoque Baixo`: Produtos cujo estoque atual está abaixo do estoque mínimo.
- `Qtd de Produtos por Trimestre`: Contagem de produtos agrupados por trimestre usando a tabela de datas.
- `Valor por Categoria`, `Valor por Produto`, `Qtd Entradas`, `Qtd Saídas`, entre outros.

---

## 🧩 Elementos do Dashboard

### Cartões

- ✅ Estoque total atual  
- 💰 Valor em estoque  
- 📦 Quantidade total de produtos  

### Gráficos

- 📊 **Estoque Atual por Categoria** (barra horizontal)  
- 🥧 **Valor por Categoria de Produto** (pizza)  
- 🏷️ **Valor por Produto** (produtos mais relevantes)  
- 🏭 **Valor por Tipo de Fornecedor** (Fábrica, Atacadista, Distribuidor)  
- 📅 **Qtd de Produtos por Trimestre** (colunas)  
- 🌍 **Filtro por Cidade** (slicer interativo)

---

## 🎯 Objetivo

Simular um sistema de Business Intelligence voltado para o setor de **logística e estoque**, que permita:

- Identificar categorias de maior impacto financeiro;
- Acompanhar níveis de estoque atual e produtos críticos;
- Analisar os fornecedores por valor de entrega;
- Observar a evolução temporal da entrada/saída de produtos;
- Interagir por filtros como cidade e categorias.

---

## 💡 Tecnologias Utilizadas

- Power BI Desktop  
- SQL Server  

---

## 📷 Screenshot do Dashboard

- 📊[Dashboard de Logística](./Imagens/Dashboard.jpg)

---

## 📬 Autor e Contato

Feito por **David Souza Ribeiro**  
📍 São Paulo - SP  
📧 [david_ribeiro2002@hotmail.com]  
🔗 [linkedin.com/in/davidsribeiro07] 

---

