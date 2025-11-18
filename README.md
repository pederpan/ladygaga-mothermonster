# ENEM_CategorizacaoQuestoes_PreTratamento
Projeto para categorização das questões do ENEM de acordo com os descritores e habilidades previstas na matriz de referência do exame.  
Este repositório faz parte de um projeto com subsistemas distribuído.  

Repositório Geral:  
https://github.com/AlexandreNP9/ENEM_CategorizacaoQuestoes_GERAL

# Objetivos deste repositório
Utilizar a API do Google Flash 2.5 com OCR  
Extrair conteúdo das questões já tratadas do ENEM  
Nas questões que contém figuras, a OCR descreve a figura.

# Especifidades técnicas
## Programas e bibliotecas
Linux Mint 22.1  
Python 3  
Gemini 2.5 flash

# Antes de executar o código
Espera-se que já tenha o python3 instalado

## Criar variável de ambiente (caso necessário)
```
python3 -m venv venv  
source venv/bin/activate  
```

## Para instalar o Google GenAI
```
pip3 install google-genai
```

## Chave API
Obter API key no Google AI Studio  
https://aistudio.google.com/app/api-keys  

Adicionar ao código na variável de ambiente com:  
```
export GEMINI_API_KEY="SUA_CHAVE_AQUI"
```

## Tenacity para tratamento de falhas
```
pip3 install tenacity
```

## Executar o script
```
python3 extrair-conteudo.py
```
