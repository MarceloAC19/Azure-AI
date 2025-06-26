# Lab Notes: Azure AI Language Studio

This document details the steps and results of the experiments conducted in the [MS Learn Text Analysis lab](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/06-text-analysis.html).

## 1. Language Detection

* **Objective:** To identify the language of a given text.
* **Sample Text:**
    ```
    I'm really enjoying this trip to Barcelona, the food is amazing.
    ```
* **Result Obtained:**
    * Language: `English`
    * Confidence Score: `0.99`
* **Observations:**
    * The model correctly identified the language with very high confidence, even with the name of a Spanish city ("Barcelona") in the middle of the sentence. The performance was excellent.

## 2. Sentiment and Opinion Analysis

* **Objective:** To identify the overall sentiment (positive, negative, neutral) and opinions about specific aspects within a text.
* **Sample Text:**
    ```
    The camera on this new phone is incredible, but the battery life is a bit disappointing. It barely lasts a full day with moderate use.
