---
title: Transformer architecture
layout: default
parent: How do LLM-s work?
nav_order: 1
---

# Transformer architecture

<p style= "padding: 35px 0px 5px;">The fundamental element of the large language models that turned out to be a game changer in the field of generative AI is the so-called <b>transformer architecture</b>. It was introduced in the paper "Attention is all you need" published in December 2017.</p>

The simplified version of the transformer architecture looks like this:

![transformer architecture simplified](TransformerArchitectureSimplified.webp)

Let's take a look at the components that make up this architecture:

- **inputs** - an input can be for example a sentence that should be translated into a different language. Since the machine learning models understand only numbers, the inputs should be encoded (= converted into a numerical format).

- **input embeddings** - input embeddings are the inputs converted into a numerical format. They function as a kind of a dictionary and help the machine learning model to understand the meaning of the words.

- **positional encoding** - positional encodings are added to the input embeddings to make sure that the original words's order is preserved. This is important because unlike former language models, the language models based on transformers, process the input embeddings not one by one but analyzes all of them at once. The main advantage of it is the fact that it decreases significantly the training time. On the other hand, though, problems with information related to words' order may occur.
