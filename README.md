# 📊 Superstore Sales Analysis

Análise exploratória e comercial baseada em dados de vendas de uma loja de varejo fictícia (Superstore).  
O objetivo deste projeto é identificar **oportunidades de melhoria de lucro**, **comportamento de vendas por região e categoria**, e **insights de desempenho**.

---

## 🎯 Objetivo do Projeto

O projeto foi desenvolvido para demonstrar habilidades práticas em:

- **Análise exploratória de dados (EDA)**  
- **Manipulação e limpeza de dados com Pandas**
- **Visualização de dados com Matplotlib e Plotly**
- **Cálculo e interpretação de métricas comerciais**

---

## ⚙️ Etapas da Análise

1. **Carregamento e limpeza dos dados**
   - Remoção de valores nulos e verificação de tipos de dados.
   - Padronização de nomes de colunas e tratamento de encoding.   

2. **Criação de métricas derivadas**
   - `Average Ticket = Sales / Quantity` (Ticket Médio)
   - `Profit Margin = (Profit / Sales) * 100` (Margem de Lucro)
   - `Cost = (Sales - Profit)` (Custo)

3. **Análise exploratória**
   - Distribuição de vendas e lucros por região e categoria.
   - Identificação de subcategorias com **lucro negativo**.
   - Avaliação do impacto dos **descontos** sobre a margem.
  
4. **Armazenamento **
   - Armazenamento, do dataset tratado, em:
      - Sqlite
      - Novo arquivo csv
      - AWS S3

6. **Visualizações**
   - Gráficos de barras (vendas e margem por região/categoria)
   - Visualização do top 5 vendas por estado        
   - Análise de perdas
   - Treemap interativo com Plotly mostrando *Sales*, *Profit* e *Average Ticket*

---

## 💡 Principais Insights

- A região **South** está por último em vendas, sugerindo oportunidade de otimização no processo de vendas e captação de clientes.
- A região **West** possui a menor margem de lucro, sugerindo oportunidade de otimização de custos ou preços.  
- Várias subcategorias como **Machines**, **Tables** e **Binders** apresentam **lucros negativos**, indicando necessidade de revisão de portfólio ou políticas de desconto.  
- O **ticket médio** é significativamente mais alto em **Technology**, refletindo maior valor agregado por produto.
- Descontos acima de 30% reduzem drasticamente a margem de lucro, indicando que promoções acima desse nível diminuem a rentabilidade da empresa.

---

## 🧰 Ferramentas Utilizadas

- **Python 3**
- **Pandas / NumPy**
- **Matplotlib / Plotly Express**
- **Boto3** (para conexão com AWS S3)
- **SQLite** (para armazenamento dos dados tratados)
- **Jupyter Notebook**

---

## 🗂️ Estrutura do Projeto
📁 superstore-analysis/  
│  
├── superstore_project.ipynb # Notebook principal  
├── data/  
│ └── superstore.csv # Dataset original  
├── output/  
│ └── superstore_clean.db # Dados tratados em SQLite  
└── README.md # Documentação do projeto  

---

## 🚀 Como Executar

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/SEU_USUARIO/superstore-analysis.git
   ```

2. **Instale as dependências:**
   ```bash
   pip install pandas numpy matplotlib plotly
   ```


3. **Execute o notebook:**
   ```bash
   jupyter notebook superstore_project.ipynb
   ```

---

## 📈 Próximos Passos

- Desenvolver um dashboard interativo com Streamlit.
- Criar pipelines automatizados de atualização de dados.

---

## 👨‍💻 Autor

**Lucas Santana**  
Desenvolvedor em transição para Engenharia de Dados

📧 lucas.hesantana16@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/lucas-hsantana/)
