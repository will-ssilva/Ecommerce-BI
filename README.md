# 📊 Projeto BI E-commerce – ETL com Python + Power BI

## 📌 Visão Geral

Este projeto simula um **pipeline completo de Business Intelligence** para um e-commerce, utilizando dados reais do Kaggle.  
O fluxo inclui **Extração, Transformação e Carga (ETL)** em Python, modelagem dimensional e criação de um dashboard interativo no **Power BI** com KPIs estratégicos.

---

## 📥 Fonte dos Dados

- **Dataset**: [E-Commerce Events History in Cosmetics Shop](https://www.kaggle.com/datasets/mkechinov/ecommerce-events-history-in-cosmetics-shop)  
- **Formato**: CSV único contendo eventos de:
  - Visualização de produtos
  - Adição ao carrinho
  - Remoção do carrinho
  - Compras

---

## ⚙️ Pipeline ETL

### 1️⃣ Extração
- Leitura do CSV original do Kaggle.

### 2️⃣ Transformação
- Conversão de datas para formato datetime.
- Criação de tabelas **dimensão** e **fato**:
  - `dim_products`
  - `dim_users`
  - `dim_date`
  - `fact_sales`
- Cálculo de métricas estratégicas (KPIs):
  - Receita Total
  - Total de Pedidos
  - Ticket Médio
  - Produtos com Maior e Menor Giro

### 3️⃣ Carga
- Exportação das tabelas tratadas para CSV.
- Disponibilização para consumo pelo Power BI.

---

## 🗃️ Modelagem Dimensional

**Modelo Star Schema**:
- **Fato**: `fact_sales` (eventos de compra)
- **Dimensões**:
  - `dim_products` (dados de produto)
  - `dim_users` (dados de cliente)
  - `dim_date` (calendário para análise temporal)

---

## 📊 Dashboard no Power BI

### **Páginas**
**Visão Geral Executiva**
![Dashboard Power BI](dashboard/preview.jpg)

## 📈 KPIs Implementados

- **Receita Total**  
- **Total de Pedidos**  
- **Ticket Médio**  

### Passos
1. Clone este repositório:
   ```bash
   git clone https://github.com/usuario/ecommerce-bi-project.git
