# Anotações do Laboratório: Azure AI Language Studio

Este documento detalha os passos e resultados dos experimentos realizados no [laboratório de Análise de Texto do MS Learn](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/10-text-analysis.html).

## 1. Detecção de Idioma

* **Objetivo:** Identificar o idioma de um determinado texto.
* **Texto de Exemplo:**
    ```
    I'm really enjoying this trip to Barcelona, the food is amazing.
    ```
* **Resultado Obtido:**
    * Idioma: `English`
    * Score de Confiança: `0.99`
* **Observações:**
    * O modelo identificou o idioma corretamente com altíssima confiança, mesmo com o nome de uma cidade espanhola ("Barcelona") no meio da frase. O desempenho foi excelente.

## 2. Análise de Sentimento e Opiniões

* **Objetivo:** Identificar o sentimento geral (positivo, negativo, neutro) e as opiniões sobre aspectos específicos em um texto.
* **Texto de Exemplo:**
    ```
    The camera on this new phone is incredible, but the battery life is a bit disappointing. It barely lasts a full day with moderate use.
    ```
* **Resultado Obtido:**
    * Sentimento Geral: `Misto (Mixed)`
    * Scores de Confiança: Positivo: `0.58`, Negativo: `0.42`, Neutro: `0.00`
* **Observações:**
    * O serviço corretamente identificou o sentimento como "Misto". Ele conseguiu associar "incredible camera" a um sentimento positivo e "disappointing battery life" a um negativo. Muito útil para análises granulares de reviews de produtos.

## 3. Extração de Frases-Chave

* **Objetivo:** Identificar os principais tópicos em um texto.
* **Texto de Exemplo:**
    ```
    Solar power is becoming a crucial component of modern energy infrastructure. Investing in photovoltaic panels can significantly reduce electricity costs for homeowners.
    ```
* **Resultado Obtido:**
    * Frases-Chave Extraídas: `Solar power`, `crucial component`, `modern energy infrastructure`, `photovoltaic panels`, `electricity costs`, `homeowners`.
* **Observações:**
    * As frases capturam perfeitamente os principais tópicos do parágrafo. A ferramenta é eficaz para resumir e indexar documentos de forma automática.

## 4. Reconhecimento de Entidades

* **Objetivo:** Identificar e categorizar entidades no texto (como pessoas, locais, organizações, datas).
* **Texto de Exemplo:**
    ```
    Satya Nadella, the CEO of Microsoft, announced a new AI initiative from their headquarters in Redmond yesterday.
    ```
* **Resultado Obtido:**
    * **Pessoa:** `Satya Nadella`
    * **Organização:** `Microsoft`
    * **Localização:** `Redmond`
    * **Data/Hora:** `yesterday`
* **Observações:**
    * O Reconhecimento de Entidades Nomeadas (NER) funcionou perfeitamente, identificando e categorizando corretamente o nome da pessoa, a empresa, a localização e a referência de tempo.
