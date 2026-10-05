---
title: "Booky: Real-Time Emotion Classification"
summary: A bidirectional LSTM trained from scratch on GoEmotions that labels the emotion of each page of a book as you read it.
tags: [NLP, Keras, BiLSTM]
github: https://github.com/DataScientistRN/BiLSTM-Emotion-Classifier-Summer-2026
icon: book
color: lavender
order: 2
---

*CSCIE-89B Introduction to Natural Language Processing · Summer 2026*

Reading is often an isolated experience. Booky imagines an e-reader that recognizes the emotions of the story alongside you.

The model is a BiLSTM built with Keras TextVectorization and Embedding layers, trained on nine emotions from the GoEmotions dataset that plausibly occur in fiction: joy, sadness, fear, anger, surprise, love, disgust, embarrassment and curiosity. A single-label and a multi-label version were compared on the same held-out test set, and the multi-label model (69% accuracy) was chosen.

It was then applied to *The Wizard of Oz*, a text it had never seen, labelling each page with an emotion and confidence score that appear at the bottom of the e-reader.
