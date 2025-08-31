# 🛠️ Manutenção Preditiva com Machine Learning

Este projeto foi desenvolvido como parte do **Bootcamp de Ciência de Dados e IA**.  
O objetivo é prever **falhas em máquinas industriais** a partir de dados IoT, identificando não só **se haverá falha**, mas também **qual tipo de falha** ocorrerá.

---

## 📊 Contexto

Empresas industriais enfrentam custos elevados com manutenção corretiva e paradas inesperadas.  
A manutenção preditiva, com apoio de **Machine Learning**, possibilita:

- Redução de falhas inesperadas  
- Aumento da eficiência operacional  
- Melhor planejamento de manutenção preventiva  

---
# Projeto de Manutenção Preditiva

Estrutura de diretórios e arquivos do projeto:

projeto_manutencao/
├── data/
│   └── bootcamp_train.csv
├── models/
│   └── (aqui serão salvos os modelos treinados, ex: random_forest.pkl)
├── src/
│   ├── __init__.py
│   ├── preprocess.py
│   ├── train.py
│   ├── avaliar.py
│   └── config.py
├── app.py
└── requisitos.txt

## 📂 Estrutura do Projeto

### 🔍 Análise Exploratória de Dados (EDA)
- Distribuições de variáveis  
- Identificação de desbalanceamento de classes  
- Correlação entre sensores e falhas  

### ⚙️ Preparação dos Dados
- Limpeza e padronização  
- Balanceamento com **SMOTE**  
- Seleção de features relevantes  

### 🤖 Modelagem
Testamos diferentes algoritmos de Machine Learning, avaliados com métricas de **Acurácia, Recall, F1-score e ROC-AUC**.  
Os três melhores modelos foram:

| Modelo          | Desempenho |
|-----------------|------------|
| 🌲 Random Forest | **0.977529** |
| 🧩 Bagging       | 0.972254   |
| 🌳 Decision Tree | 0.958237   |

➡️ O **Random Forest** foi escolhido como modelo final por apresentar o melhor equilíbrio de performance.  

### 📈 Resultados
- Modelos de ensemble (**Random Forest** e **Bagging**) se destacaram  
- Principais variáveis: **Torque, Desgaste da Ferramenta, Temperatura do Processo**  

### ✅ Conclusões e Próximos Passos
- **Impacto**: redução de paradas, segurança operacional e economia em manutenção  
- **Evolução futura**:  
  - Deploy do modelo via **FastAPI**  
  - **Dashboard interativo** (Streamlit)  
  - Deploy em **nuvem/Docker**  

---

## 📊 Principais Insights
- **Torque** e **desgaste da ferramenta** são os maiores preditores de falha  
- **Classes desbalanceadas** exigiram oversampling (**SMOTE**)  
- Melhor modelo final (**Random Forest**) atingiu **alta performance (0.9775)**, balanceando bem **Recall e F1-score**  

---

## 🚀 Tecnologias Utilizadas
- Python (Pandas, Numpy, Scikit-learn, Imbalanced-learn, Seaborn, Matplotlib)  
- Ydata-profiling (para EDA automatizada)  
- Algoritmos de Machine Learning (Scikit-learn)  



