""# 📌 Leitura de Planilhas do Google Sheets com Google Colab

## 📄 **Descrição do Projeto**

Este projeto demonstra como realizar a leitura de planilhas hospedadas no **Google Sheets** diretamente no **Google Colab** utilizando o módulo `pandas`. A integração é feita através da exportação das planilhas no formato CSV, permitindo o carregamento remoto dos dados para análise e manipulação de forma simples e prática.

---

## ✅ **Pré-requisitos**

* Conta Google para acesso às planilhas.
* Planilha publicada para acesso via link compartilhável.
* Permissões de leitura pública ou compartilhamento adequado.

---

## 🚀 **Como Executar**

1. Clone o repositório:

   ```bash
   git clone https://github.com/brodyandre/Leitura-Google-Sheets-Colab.git
   ```

2. Acesse o Google Colab e faça o upload do arquivo `.ipynb` do projeto.

3. Execute as células sequencialmente para ler os dados das planilhas.

---

## ⚙️ **Funcionalidades**

* Leitura de planilhas públicas do Google Sheets.
* Visualização inicial dos dados com `head()`.
* Carregamento de diferentes abas do Google Sheets de forma dinâmica.

---

## 💡 **Exemplos de Uso**

### **1️⃣ Leitura da planilha de emissões de CO2**

```python
import pandas as pd

# Definindo o ID da planilha
sheet_id = '1pvBoLyX8kP0TjtUbadVMGdTl4yzm6bHMThhPiqCVtpw'

# Montando a URL para leitura
url = f'https://docs.google.com/spreadsheets/d/{sheet_id}/gviz/tq?tqx=out:csv&sheet'

# Lendo os dados
dados_co2_sheet = pd.read_csv(url)

# Visualizando as 5 primeiras linhas
dados_co2_sheet.head()
```

### **2️⃣ Leitura da planilha de emissões per capita**

```python
# Nome da aba que desejamos acessar
sheet_name = 'emissoes_percapita'

# Montando a URL para leitura
url_percapita = f'https://docs.google.com/spreadsheets/d/{sheet_id}/gviz/tq?tqx=out:csv&sheet={sheet_name}'

# Lendo os dados
percapita_sheets = pd.read_csv(url_percapita)

# Visualizando as 5 primeiras linhas
percapita_sheets.head()
```

### **3️⃣ Leitura da planilha de fontes de emissão**

```python
# Nome da aba que desejamos acessar
sheet_name = 'fontes'

# Montando a URL para leitura
url_fontes = f'https://docs.google.com/spreadsheets/d/{sheet_id}/gviz/tq?tqx=out:csv&sheet={sheet_name}'

# Lendo os dados
fontes_sheets = pd.read_csv(url_fontes)

# Visualizando as 5 primeiras linhas
fontes_sheets.head()
```

---

## 🛠️ **Tecnologias Utilizadas**

* Python 3.9+
* Pandas
* Google Colab

---

## 🤝 **Contribuição**

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar PRs para melhorias.

---

## 📜 **Licença**

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 🔗 **Contato**

Luiz André de Souza - [LinkedIn](https://www.linkedin.com/in/luizandre)
GitHub: [brodyandre](https://github.com/brodyandre)
""

