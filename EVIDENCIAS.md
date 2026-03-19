# 📡 Evidências do Projeto LGPD Data Mapper

Este documento apresenta, de forma estruturada, as evidências da execução do projeto **LGPD Data Mapper**, demonstrando todas as etapas desde a criação do ambiente até a geração do relatório final.

---

## 🖥️ Environment Setup

Nesta etapa foi realizada a criação do ambiente de desenvolvimento no Kali Linux, incluindo a estrutura inicial do projeto e organização dos diretórios.

### 🔧 Comandos executados:

```bash
mkdir lgpd-data-mapper
cd lgpd-data-mapper
mkdir data reports
```

### 💬 Descrição:
- Criação do diretório principal do projeto  
- Acesso à pasta do projeto  
- Criação das pastas `data` (entrada) e `reports` (saída)  

📸 Evidência:  
<img width="1920" height="936" alt="Environment Setup" src="https://github.com/user-attachments/assets/c85921f1-fc7c-4242-8c83-409cdbd204b3" />

---

## 📝 Criação do Arquivo de Entrada

Foi criado um arquivo contendo dados simulados para teste, incluindo informações pessoais e sensíveis.

### 🔧 Comando executado:

```bash
nano data/input.txt
```

### 💬 Descrição:
Arquivo de entrada contendo exemplos de:
- CPF  
- E-mail  
- Telefone  
- Dados sensíveis (saúde, religião)  

📸 Evidência:  
<img width="1920" height="936" alt="Input File" src="https://github.com/user-attachments/assets/a1ade544-2c7a-4c2d-bf5f-1898deaa2e27" />

---

## 💻 Desenvolvimento do Código

Nesta etapa foram desenvolvidos os scripts responsáveis pela análise e classificação dos dados.

### 📌 Arquivo: `mapper.py`

### 💬 Função:
- Identificação de dados pessoais utilizando Regex  
- Detecção de dados sensíveis no conteúdo analisado  

📸 Evidência:  
<img width="1920" height="936" alt="mapper.py" src="https://github.com/user-attachments/assets/c5ef9e1d-f15e-428b-bfa3-e30d8f300874" />

---

### 📌 Arquivo: `main.py`

### 💬 Função:
- Leitura do arquivo de entrada  
- Processamento dos dados  
- Geração do relatório em JSON  

📸 Evidência:  
<img width="1920" height="936" alt="main.py" src="https://github.com/user-attachments/assets/a807f604-75c3-40fa-a584-0c89525678c0" />

---

## 🚀 Execução do Script

O script principal foi executado no terminal para processar os dados.

### 🔧 Comando executado:

```bash
python3 main.py
```

### 💬 Resultado:
- Leitura dos dados de entrada  
- Identificação automática de informações pessoais  
- Classificação de dados sensíveis  

📸 Evidência:  
<img width="1920" height="936" alt="Execução do Script" src="https://github.com/user-attachments/assets/2e1570ec-9ce0-4da1-acc0-1c76ca846cb5" />

---

## 📊 Resultado Gerado

Após a execução, foi gerado um arquivo estruturado em JSON contendo os dados identificados.

### 🔧 Comando executado:

```bash
cat reports/resultado.json
```

### 💬 Descrição:
O arquivo gerado apresenta:
- Dados pessoais organizados por categoria  
- Lista de dados sensíveis identificados  

📸 Evidência:  
<img width="1920" height="936" alt="Resultado JSON" src="https://github.com/user-attachments/assets/36bebdf4-3c1c-414d-b9d4-14f0d2d61a7c" />

---

## ✅ Conclusão

Os resultados demonstram a capacidade do sistema em identificar e classificar dados pessoais e sensíveis de forma automatizada.

Este projeto evidencia a aplicação prática de conceitos de:
- LGPD  
- Cibersegurança  
- Análise de dados  

Podendo ser expandido para cenários mais avançados, como auditorias automatizadas e integração com sistemas corporativos.
