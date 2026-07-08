# 📄 Emissão de Nota Fiscal Automatizada

Automação em Python que simula o processo de emissão de notas fiscais para uma base de clientes, utilizando **Selenium** para interação com o navegador e **Pandas** para manipulação de dados.

## 🎯 Objetivo

Simular um cenário real de RPA (Robotic Process Automation): eliminar o preenchimento manual e repetitivo de formulários de emissão de nota fiscal, reduzindo tempo e risco de erro humano.

## ⚙️ Como funciona

1. O robô abre o navegador e acessa a tela de login do sistema (`login.html`)
2. Faz login automaticamente com as credenciais configuradas
3. Lê a base de clientes fictícia (`NotasEmitir.xlsx`) usando **pandas**
4. Para cada cliente da planilha, preenche automaticamente o formulário de emissão de NF (`index.html`): nome, endereço, bairro, município, CEP, UF, CPF/CNPJ, inscrição estadual, descrição, quantidade e valores
5. Clica no botão de emissão e recarrega a página para processar o próximo cliente
6. Repete o processo até finalizar toda a base

## 🛠️ Tecnologias utilizadas

- Python
- Selenium
- Pandas
- WebDriver Manager
- HTML (sistema fictício de login e emissão de NF)

## 📂 Estrutura do projeto
├── EmissaoNF.ipynb       # Script principal da automação
├── login.html            # Tela de login fictícia
├── index.html            # Formulário de emissão de nota fiscal
├── NotasEmitir.xlsx      # Base de clientes fictícia
├── requirements.txt      # Dependências do projeto
└── README.md
## ▶️ Como executar

```bash
# Clone o repositório
git clone https://github.com/ViniciusCavalcanti-03/emissao-nf-selenium.git

# Instale as dependências
pip install -r requirements.txt

# Execute o notebook EmissaoNF.ipynb
```

## 👤 Autor

**Vinicius Cavalcanti Vilela Lins**
[LinkedIn](www.linkedin.com/in/vinicius-cavalcanti-si) | [GitHub](https://github.com/ViniciusCavalcanti-03)

> ⚠️ Projeto desenvolvido para fins de estudo. Todos os dados de clientes utilizados são fictícios.
