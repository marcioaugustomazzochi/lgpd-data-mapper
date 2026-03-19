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
- `mkdir lgpd-data-mapper` → cria o diretório do projeto  
- `cd lgpd-data-mapper` → acessa a pasta criada  
- `mkdir data reports` → cria diretórios para entrada e saída de dados  

📸 Evidência:  
<img width="1920" height="936" alt="Environment Setup" src="https://github.com/user-attachments/assets/c85921f1-fc7c-4242-8c83-409cdbd204b3" />

---

## 📝 Criação do Arquivo de Entrada

Foi criado um arquivo contendo dados simulados para teste, incluindo informações pessoais e sensíveis.

### 🔧 Comando utilizado:

```bash
nano data/input.txt
```

### 💬 Descrição:
Arquivo utilizado como base para análise, contendo exemplos como:
- CPF  
- E-mail  
- Telefone  
- Dados sensíveis (saúde, religião)

📸 Evidência:  
<img width="1920" height="936" alt="Input File" src="https://github.com/user-attachments/assets/a1ade544-2c7a-4c2d-bf5f-1898deaa2e27" />

---

## 💻 Desenvolvimento do Código

Nesta etapa foram implementados os scripts responsáveis pela leitura, análise e classificação dos dados.

### 📌 Arquivo: `mapper.py`

### 💬 Função:
Responsável por:
- Identificar padrões de dados pessoais via Regex  
- Detectar dados sensíveis no texto  

📸 Evidência:  
<img width="1920" height="936" alt="mapper.py" src="https://github.com/user-attachments/assets/c5ef9e1d-f15e-428b-bfa3-e30d8f300874" />

---

### 📌 Arquivo: `main.py`

### 💬 Função:
- Executa o processo de leitura do arquivo  
- Chama o mapper  
- Gera o relatório final em JSON  

📸 Evidência:  
<img width="1920" height="936" alt="main.py" src="https://github.com/user-attachments/assets/a807f604-75c3-40fa-a584-0c89525678c0" />

---

## 🚀 Execução do Script

O script principal foi executado no terminal para processar os dados.

### 🔧 Comando executado:

```bash
python3 main.py
```

### 💬 Resultado esperado:
- Leitura do arquivo de entrada  
- Identificação dos dados  
- Exibição do resultado no terminal  

📸 Evidência:  
<img width="1920" height="936" alt="Execução do Script" src="https://github.com/user-attachments/assets/2e1570ec-9ce0-4da1-acc0-1c76ca846cb5" />

---

## 📊 Resultado Gerado

Após a execução, foi gerado um arquivo estruturado em JSON contendo os dados identificados.

### 🔧 Comando utilizado:

```bash
cat reports/resultado.json
```

### 💬 Descrição:
O arquivo apresenta:
- Dados pessoais organizados por tipo  
- Lista de dados sensíveis identificados  

📸 Evidência:  
<img width="1920" height="936" alt="Resultado JSON" src="https://github.com/user-attachments/assets/36bebdf4-3c1c-414d-b9d4-14f0d2d61a7c" />

---

## ✅ Conclusão

Os resultados demonstram a capacidade do sistema em identificar e classificar dados pessoais e sensíveis de forma automatizada.

O projeto evidencia a aplicação prática de conceitos de:
- LGPD  
- Cibersegurança  
- Análise de dados  

Podendo ser expandido para cenários mais robustos, como auditorias automatizadas e integração com sistemas corporativos.
