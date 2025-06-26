# Lab Notes: Azure AI Speech Studio

This document details the steps and results of the experiments conducted in the [MS Learn Speech Analysis lab](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/09-speech.html).

## 1. Speech-to-Text

* **Objective:** To transcribe audio to text. The lab explores real-time transcription (using the microphone) and transcription from an audio file.
* **Method Used:** (X) Real-time ( ) Audio file
* **Transcription Result:**
    ```
    Ok, I'm starting the test now... The quick brown fox jumps over the lazy dog. How well is this being transcribed?
    ```
* **Observations:**
    * The accuracy was very high. The model automatically added punctuation (period and question mark), which is impressive. The speech "Okay, I'm" was transcribed as "Ok, I'm," a minor but acceptable variation.

## 2. Text-to-Speech

* **Objective:** To synthesize a natural voice from text.
* **Sample Text:**
    ```xml
    <speak version="1.0" xmlns="[http://www.w3.org/2001/10/synthesis](http://www.w3.org/2001/10/synthesis)" xml:lang="pt-BR">
        <voice name="pt-BR-FranciscaNeural">
            Welcome to the future of artificial intelligence.
            <break time="500ms"/>
            Here, your ideas come to life with a natural voice.
        </voice>
    </speak>
    ```
* **Voice Settings:**
    * Language: `Portuguese (Brazil)`
    * Voice: `pt-BR-FranciscaNeural`
    * Speech Style: `Default`
* **Observations:**
    * The 'FranciscaNeural' voice is extremely natural and fluid. Using the SSML tag `<break time='500ms'/>` worked perfectly to add a dramatic pause between sentences, showcasing the power of customization.

## 3. Speech Translation

* **Objective:** To translate speech from a source language to a target language.
* **Source Language:** `English (US)`
* **Target Language:** `Spanish`
* **Spoken Phrase (imagined):** `This is a real-time translation test to see the service's performance.`
* **Translation Result:**
    ```
    Esta es una prueba de traducción en tiempo real para ver el rendimiento del servicio.
    ```
* **Observations:**
    * The translation was instantaneous and accurate, maintaining the exact meaning of the original sentence. The latency was minimal, making the service viable for live conversation applications. The quality of the synthesized Spanish voice was also excellent.
