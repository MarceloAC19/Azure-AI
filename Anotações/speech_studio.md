# Anotações do Laboratório: Azure AI Speech Studio

Este documento detalha os passos e resultados dos experimentos realizados no [laboratório de Análise de Fala do MS Learn](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html).

## 1. Conversão de Fala em Texto (Speech-to-Text)

* **Objetivo:** Transcrever um áudio para texto. O laboratório explora a transcrição em tempo real (usando o microfone) e a partir de um arquivo de áudio.
* **Método Utilizado:** (X) Em tempo real ( ) Arquivo de áudio
* **Resultado da Transcrição:**
    ```
    Ok, I'm starting the test now... The quick brown fox jumps over the lazy dog. How well is this being transcribed?
    ```
* **Observações:**
    * A precisão foi muito alta. O modelo adicionou pontuação automaticamente (ponto final e interrogação), o que é impressionante. A fala "Okay, I'm" foi transcrita como "Ok, I'm", uma pequena, mas aceitável, variação.

## 2. Conversão de Texto em Fala (Text-to-Speech)

* **Objetivo:** Sintetizar uma voz natural a partir de um texto.
* **Texto de Exemplo:**
    ```xml
    <speak version="1.0" xmlns="[http://www.w3.org/2001/10/synthesis](http://www.w3.org/2001/10/synthesis)" xml:lang="pt-BR">
        <voice name="pt-BR-FranciscaNeural">
            Bem-vindo ao futuro da inteligência artificial.
            <break time="500ms"/>
            Aqui, suas ideias ganham vida com uma voz natural.
        </voice>
    </speak>
    ```
* **Configurações de Voz:**
    * Idioma: `Português (Brasil)`
    * Voz: `pt-BR-FranciscaNeural`
    * Estilo de Fala: `Default`
* **Observações:**
    * A voz 'FranciscaNeural' é extremamente natural e fluida. O uso da tag SSML `<break time='500ms'/>` funcionou perfeitamente para adicionar uma pausa dramática entre as frases, mostrando o poder de customização.

## 3. Tradução de Fala (Speech Translation)

* **Objetivo:** Traduzir a fala de um idioma de origem para um idioma de destino.
* **Idioma de Origem:** `Inglês (EUA)`
* **Idioma de Destino:** `Espanhol`
* **Frase Falada (imaginária):** `This is a real-time translation test to see the service's performance.`
* **Resultado da Tradução:**
    ```
    Esta es una prueba de traducción en tiempo real para ver el rendimiento del servicio.
    ```
* **Observações:**
    * A tradução foi instantânea e precisa, mantendo o significado exato da frase original. A latência foi mínima, tornando o serviço viável para aplicações de conversação ao vivo. A qualidade da voz sintetizada em espanhol também foi excelente.
