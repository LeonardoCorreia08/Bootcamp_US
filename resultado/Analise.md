# 🔍 Análise Exploratória de Dados (EDA)

A etapa de **Análise Exploratória de Dados (EDA)** foi essencial para compreender a base utilizada no projeto de manutenção preditiva.  
O estudo revelou **padrões, relações entre variáveis e desafios importantes**, como o desbalanceamento das classes.

---

## 📊 Correlação entre Variáveis

Foi observado que algumas variáveis apresentam **forte correlação**, especialmente entre os atributos **mecânicos**:

- Torque e Velocidade Rotacional possuem alta dependência.  
- Potência Mecânica também acompanha essas variáveis, reforçando sua relevância no processo.  

![Correlação entre Sensores](assets/correlacoes.png)  
*<p align="center">Mapa de calor destacando as correlações entre variáveis numéricas.</p>*  

---

## ⚖️ Distribuição de Classes

Outro ponto crítico identificado foi o **desbalanceamento das classes**.  
A classe **"sem falha" (0)** representa a grande maioria dos registros, enquanto os casos de **"falha" (1)** são bem menos frequentes.

- Isso torna a modelagem mais desafiadora, pois modelos ingênuos tenderiam a prever apenas a classe majoritária.  
- Estratégias de **balanceamento** (como oversampling/undersampling ou ajustes de peso nas classes) se tornam necessárias para evitar viés.  

![Distribuição de Falhas](assets/DistribuiçãodeFalhasdaMáquinaportipo.png)  
*<p align="center">Distribuição de classes: predominância de registros "sem falha".</p>*  

---

## ✅ Insights Gerais

1. **Variáveis Mecânicas** (torque, rotação, potência) são as que mais se relacionam com possíveis falhas.  
2. **Variáveis Ambientais** (temperatura do ar, umidade) apresentam impacto limitado, mas podem atuar como fatores secundários.  
3. **Desbalanceamento de Classes** exige atenção especial na escolha de métricas (F1-Score, Recall) e técnicas de modelagem.  
4. A base de dados mostra-se adequada para aplicação de **modelos supervisionados**, desde que o desbalanceamento seja tratado.  

---

📌 Essa análise inicial guiou a modelagem, ajudando a priorizar variáveis e selecionar métricas adequadas para o problema de manutenção preditiva.
