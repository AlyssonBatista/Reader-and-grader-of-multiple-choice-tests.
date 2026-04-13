# 📄 Multiple Choice Test Reader & Grader

Sistema automatizado para leitura e correção de provas de múltipla escolha a partir de imagens, utilizando técnicas de visão computacional e processamento de imagens em Python.

---

## 📌 Sobre o Projeto

Este projeto tem como objetivo identificar e corrigir automaticamente cartões de resposta (answer sheets) de provas objetivas.

Através do notebook `Answer_Sheet.ipynb`, o sistema:

- Processa imagens de folhas de respostas
- Detecta marcações feitas pelo candidato
- Identifica alternativas selecionadas
- Compara com um gabarito previamente definido
- Calcula a pontuação final

Esse tipo de abordagem utiliza OMR (Optical Mark Recognition), técnica usada para reconhecer marcações em formulários.

---

## ⚙️ Tecnologias Utilizadas

- Python 3
- OpenCV
- NumPy
- Matplotlib (opcional)
- Jupyter Notebook

---

## 🚀 Funcionalidades

- 📷 Leitura de imagens de cartões de resposta  
- 🔍 Detecção de contornos e regiões de interesse  
- ✏️ Identificação de bolhas marcadas  
- ✅ Correção automática com base no gabarito  
- 📊 Cálculo de nota final  
- 🧪 Visualização do processamento (modo debug)  

---

## 🧠 Como Funciona

O sistema segue o seguinte fluxo:

### 1. Pré-processamento da imagem
- Conversão para escala de cinza
- Aplicação de blur para redução de ruído
- Binarização (threshold)

### 2. Detecção da folha
- Identificação de contornos principais
- Correção de perspectiva (transformação da imagem)

### 3. Segmentação das questões
- Divisão da imagem em regiões correspondentes às perguntas

### 4. Detecção de respostas
- Identificação das bolhas preenchidas
- Análise da intensidade de pixels

### 5. Correção
- Comparação com o gabarito
- Cálculo da pontuação final

---

## 📂 Estrutura do Projeto
