# Desafio de Ciência de Dados - Precificação de Aluguéis

<div align="center">
  <img src="cover.png" width="100%" alt="Capa do Projeto">
</div>

Repositório para resolução de problemas de negócios, análise de dados e aplicação de modelos preditivos diversos em machine learning.

## 📌 Sobre o Projeto
Este projeto tem como objetivo desenvolver um modelo de previsão de preços de aluguéis temporários na cidade de Nova York, utilizando dados de um concorrente como referência. A solução envolve análise exploratória dos dados (EDA), modelagem preditiva e avaliação de desempenho. 

## 🛠 Tecnologias Utilizadas
- Python 3.x
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib & Seaborn
- Joblib

## 📂 Estrutura do Repositório
```
├── LH_CD_FabioNogueira.ipynb   # Notebook com a análise e modelagem
├── modelo_precificacao.pkl      # Modelo treinado salvo
├── teste_indicium_precificacao.csv  # Dataset utilizado
├── requirements.txt            # Lista de dependências
└── README.md                   # Este arquivo
```

## 🚀 Como Instalar e Executar

### 1️⃣ Clonar o Repositório
```bash
git clone <URL_DO_REPOSITORIO>
cd <NOME_DO_REPOSITORIO>
```

### 2️⃣ Criar e Ativar um Ambiente Virtual
```bash
python -m venv venv
# Ativar ambiente virtual
# No Windows:
venv\Scripts\activate
# No macOS/Linux:
source venv/bin/activate
```

### 3️⃣ Instalar as Dependências
```bash
pip install -r requirements.txt
```

### 4️⃣ Executar o Notebook
Abra o Jupyter Notebook e execute `LH_CD_FabioNogueira.ipynb`
```bash
jupyter notebook
```

### 5️⃣ Fazer Previsões com o Modelo Treinado
Para carregar o modelo salvo e fazer previsões:
```python
import joblib
import pandas as pd

# Carregar modelo
modelo = joblib.load('modelo_precificacao.pkl')

# Criar um exemplo de entrada
entrada = pd.DataFrame({
    'bairro_group': ['Manhattan'],
    'bairro': ['Midtown'],
    'latitude': [40.75362],
    'longitude': [-73.98377],
    'room_type': ['Entire home/apt'],
    'minimo_noites': [1],
    'numero_de_reviews': [45],
    'calculado_host_listings_count': [2],
    'disponibilidade_365': [355]
})

# Fazer a previsão do preço
y_pred = model.predict(X_test)
print(f'Preço previsto: ${y_pred[0]:.2f}')
```

## 📩 Contato
Atividade realizada por **Fábio Nogueira**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-1B1C1E?style=for-the-badge&logo=linkedin&logoColor=0077B5&border_color=fcf901)](https://www.linkedin.com/in/faanogueira/)
[![GitHub](https://img.shields.io/badge/GitHub-1B1C1E?style=for-the-badge&logo=linkedin&logoColor=0077B5&border_color=fcf901)](https://github.com/faanogueira)
[![Gmail](https://img.shields.io/badge/Gmail-1B1C1E?style=for-the-badge&logo=gmail&logoColor=C71610)](mailto:faanogueira@gmail.com)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-1B1C1E?style=for-the-badge&logo=whatsapp&logoColor=green)](https://api.whatsapp.com/send?phone=5571983937557)

