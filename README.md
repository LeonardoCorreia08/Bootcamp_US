# 🔧 Manutenção Preditiva com Machine Learning

Projeto desenvolvido como parte do **Bootcamp de Ciência de Dados e IA**.  
O objetivo é construir um pipeline de ponta a ponta para prever **falhas em máquinas industriais** a partir de dados de sensores, possibilitando a atuação **proativa** da equipe de manutenção.

---

## 📊 Contexto do Negócio

Empresas industriais enfrentam custos elevados com **manutenção corretiva** e **paradas inesperadas** de produção.  
A manutenção preditiva, apoiada por **Machine Learning**, surge como solução estratégica para:

- 🚫 Reduzir o número de falhas inesperadas.  
- ⚡ Aumentar a eficiência e a vida útil dos equipamentos.  
- 📅 Otimizar o planejamento de paradas para manutenção.  
- 💰 Reduzir custos operacionais e de reparo.  

---

## 📖 Acesso Rápido

- [📂 Estrutura do Projeto](#-estrutura-do-projeto)  
- [🔧 Ferramentas](#-ferramentas)  
- [⚡ Pipeline Principal](#️-executar-o-pipeline-principal)  
- [📉 Percurso Analítico](#-percurso-analítico)  
  

---

## 📂 Estrutura do Projeto

O código foi organizado de forma **modular**, garantindo clareza, escalabilidade e fácil manutenção.

![Estrutura do Projeto](assets/estrutura.PNG)

---

# 🔧Ferramenta

## Como Executar o Projeto

Siga os passos abaixo para configurar o ambiente e executar o pipeline completo de treinamento e avaliação.


## ✅ Pré-requisitos

- Python **3.9 ou superior**  
- `pip` (gerenciador de pacotes do Python)  
---

## 📂 Clonar o Repositório

### A. Clona o repositório para uma pasta chamada "Bootcamp_US"
```bash
git clone https://github.com/LeonardoCorreia08/Bootcamp_US.git
```
### B. Entra na pasta que acabou de ser criada
```
cd Bootcamp_US
```
## Passos para Execução
```
Criar um Ambiente Virtual (Recomendado)
```
### Cria o ambiente virtual
```
python -m venv venv
```
### Ativa o ambiente (Linux/macOS)
```
source venv/bin/activate
```
### Ativa o ambiente (Windows)
```
.\venv\Scripts\activate
```

### Instalar as Dependências
O arquivo requirement.txt contém todas as bibliotecas necessárias.
```
pip install -r requirement.txt
```
### Inicializar o Projeto

📌 Para rodar o pipeline completo, basta executar:
```bash
python main.py
```
✅ Pronto! O ambiente estará configurado e o projeto inicializado corretamente.

### Executar o Pipeline Principal

O script `main.py` é responsável por **orquestrar todo o pipeline de Machine Learning**.  
Ao executá-lo, as seguintes etapas são realizadas automaticamente, de forma sequencial:

1. **Configuração** – Carregamento dos parâmetros do projeto.  
2. **Pré-processamento** – Limpeza, transformação e balanceamento dos dados.  
3. **Treinamento** – Treino do modelo de Machine Learning definido.  
4. **Avaliação** – Cálculo das métricas de performance (Accuracy, F1, etc.) e geração de relatórios.  
5. **Persistência** – Salvamento do modelo final em `models/` para uso futuro (API, dashboards, etc.).

✅ Isso garante que todas as etapas — configuração → pré-processamento → treino → avaliação → salvamento — sejam executadas em um único fluxo contínuo.

---

### Docker
Docker é uma plataforma de contêinerização que permite criar, implantar e executar aplicativos em contêineres. É amplamente utilizado para garantir que os ambientes de desenvolvimento e produção sejam consistentes.

- **Principais Características**: Portabilidade, consistência de ambiente, isolamento de aplicativos.
- **Casos de Uso**: Implantação de aplicações, isolamento de ambientes de desenvolvimento.
- **Links**:
- [Docker Official Site](https://www.docker.com/)
- [Docker Documentation](https://docs.docker.com/)

Se estiver utilizando Windows, você pode inicializar rapidamente com o script:
```
QUICK-START-Windows.bat
```

# Percurso Analítico

[Análise Exploratória](https://github.com/LeonardoCorreia08/Bootcamp_US/blob/main/resultado/Analise.md)

[Relatório](https://github.com/LeonardoCorreia08/Bootcamp_US/blob/main/)



---

---

## 💻 Tecnologias Utilizadas

- **Linguagem**: Python  
- **Bibliotecas**: Pandas, Numpy, Scikit-learn, Imbalanced-learn, Seaborn, Matplotlib  
- **Análise Exploratória**: Ydata-profiling  
