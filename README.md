# 📊 Análise de Dados – Locadora de Filmes (Sakila)

## 📌 Visão Geral
Este projeto tem como objetivo analisar o desempenho financeiro de uma locadora de filmes utilizando o banco de dados **Sakila** (MySQL Sample Database).  
A análise foi conduzida com **SQL** para modelagem e transformação dos dados e **Power BI** para visualização e geração de insights de negócio.

O foco do projeto é responder perguntas reais de negócio por meio de **análise exploratória**, **modelagem dimensional** e **dashboards interativos**.

---
## 📈 Dashboard
O dashboard foi desenvolvido no Power BI com foco em clareza visual e insights de negócio.

<img width="1511" height="845" alt="dashboard" src="https://github.com/user-attachments/assets/a9ce6477-31d9-483b-ada0-c2f387648e86" />

Principais visualizações:
- Receita total
- Receita por filme
- Receita por categoria
- Receita por cliente
- Receita por loja
- Evolução mensal da receita

---

## ❓ Perguntas de Negócio Respondidas
- Qual é a **receita total** da locadora e sua **evolução ao longo do tempo**?
- Quais **filmes geram mais receita**?
- Quais **categorias concentram o maior faturamento**?
- Qual **loja apresenta melhor desempenho financeiro**?
- A receita está **concentrada em poucos clientes** ou bem distribuída?

---

## 🔎 Principais Insights
- A locadora apresentou uma receita total acumulada de 67.406,56 no período analisado.
Observa-se um pico expressivo de faturamento em julho de 2005, ultrapassando 20 mil em receita. Após esse período, ocorre uma queda contínua e acentuada, chegando a valores próximos de zero em janeiro de 2006, o que pode indicar sazonalidade, redução de demanda ou encerramento gradual das operações.

- A receita está concentrada em poucos títulos, com destaque para TELEGRAPH VOYAGE (232), WIFE TURN (224) e ZORRO ARK (215). Esses filmes se destacam como principais responsáveis pelo faturamento, sugerindo oportunidades para estratégias como maior divulgação ou priorização de estoque.

- As categorias com maior geração de receita são Sports (5.314), Sci-Fi (4.757) e Animation (4.656). Essas categorias concentram grande parte do faturamento, indicando preferência clara dos clientes e possível direcionamento para decisões de catálogo e investimento.

- A análise dos 5 principais clientes mostra uma distribuição relativamente uniforme da receita, variando de 222 a 195. Isso indica que, mesmo entre os maiores consumidores, não há forte dependência de um único cliente, reduzindo riscos associados à concentração de receita.

- O desempenho financeiro entre as lojas é bastante equilibrado. A Loja 2 apresenta faturamento levemente superior (33.726,77) em comparação à Loja 1 (33.679,79). A diferença é pequena, sugerindo consistência operacional entre as unidades.
---

## 🛠️ Tecnologias Utilizadas
- **MySQL** (SQL)
- **Power BI**
- **Modelagem Dimensional (Esquema Estrela)**

---

## 🗂️ Modelagem de Dados
Os dados foram organizados utilizando um **modelo estrela**, facilitando a análise no Power BI.

### 🔹 Tabela Fato
- **fato_vendas**
  - customer_id
  - film_id
  - category_id
  - store_id
  - amount
  - payment_date

### 🔹 Tabelas Dimensão
- **dim_cliente** (dados do cliente)
- **dim_filme** (título do filme)
- **dim_categoria** (categoria do filme)

Essa modelagem permite análises eficientes de receita por tempo, cliente, filme, categoria e loja.

---

## 📚 Fonte dos Dados
- **Sakila Database** – MySQL Sample Database
