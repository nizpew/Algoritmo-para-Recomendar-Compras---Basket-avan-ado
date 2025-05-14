
## 🛒 Recomendação de Compras em Cesta com Regras de Associação

### 📌 Descrição

Este projeto demonstra como aplicar técnicas de **Data Mining** com **Regras de Associação** para identificar padrões de compra em dados transacionais de supermercado. Utilizamos o dataset público **Groceries Dataset** (Kaggle) para extrair **insights valiosos sobre o comportamento de compra dos clientes**, como itens frequentemente comprados juntos e oportunidades de promoções cruzadas.

A base teórica inclui os algoritmos **Apriori** e o uso de métricas como **suporte**, **confiança** e **lift**.

---

### 📊 Objetivos

* Descobrir **padrões ocultos** nas transações.
* Gerar **regras de associação** usando o algoritmo Apriori.
* Identificar **oportunidades de marketing**, como produtos frequentemente comprados juntos.
* Simular como sistemas de recomendação (como os da Amazon ou Mercado Livre) funcionam com base em itens comprados em conjunto.

---

### 📁 Dataset

* **Fonte**: Kaggle – [`heeraldedhia/groceries-dataset`](https://www.kaggle.com/datasets/heeraldedhia/groceries-dataset)
* **Formato**: CSV
* **Colunas**:

  * `Member_number`: ID do cliente
  * `Date`: data da compra
  * `itemDescription`: produto comprado

---

### ⚙️ Tecnologias e Bibliotecas

* Python 3
* Pandas
* mlxtend (para Apriori e regras de associação)
* KaggleHub (para carregar datasets do Kaggle)
* Matplotlib / Seaborn (opcional para visualizações)
* tabulate (para exibir tabelas formatadas)

---

### 🚀 Como Executar

1. Clone o repositório:

   ```bash
   git clone https://github.com/seuusuario/market-basket-analysis.git
   cd market-basket-analysis
   ```

2. Instale as dependências:

   ```bash
   pip install pandas mlxtend kagglehub tabulate
   ```

3. Execute o script Jupyter ou `.py` com seu ambiente Python favorito.

---

### 🔍 Resultados

#### 📈 Top 10 Produtos Mais Frequentes

| Produto          | Suporte (%) |
| ---------------- | ----------- |
| whole milk       | 15.7        |
| other vegetables | 12.2        |
| rolls/buns       | 11.0        |
| soda             | 9.7         |
| yogurt           | 8.5         |

#### 📋 Top 5 Regras de Associação

| Antecedente | Consequente | Lift | Confiança |
| ----------- | ----------- | ---- | --------- |
| curd        | sausage     | 1.45 | 8.7%      |
| brown bread | canned beer | 1.36 | 6.3%      |
| sausage     | curd        | 1.45 | 4.8%      |

#### 🎯 Resumo Visual para Apresentação:

| Insight                            | Ação Recomendável               |
| ---------------------------------- | ------------------------------- |
| Whole milk é o item mais frequente | Destaque na loja/app            |
| curd → sausage (lift 1.45)         | Promoção cruzada                |
| brown bread → canned beer          | Sugestão no carrinho            |
| sausage é central em várias regras | Produto-chave para estratégias  |
| Vegetais + frankfurter             | Perfil misto: saudável + rápido |

---

### 📚 Conceitos Envolvidos

* **Regras de Associação**: Identificação de produtos frequentemente comprados em conjunto.
* **Apriori Algorithm**: Algoritmo para encontrar itemsets frequentes de forma eficiente.
* **Lift**: Mede o quão mais provável é a compra conjunta em comparação ao acaso.

---

### 📌 Aplicações Reais

* Recomendação de produtos em e-commerces.
* Promoções cruzadas e planejamento de layout em supermercados.
* Análise de comportamento do consumidor.

---

