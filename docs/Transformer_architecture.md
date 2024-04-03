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

- **inputs** - an input can be for example a sentence that should be translated into a different language. 
  
  Since the machine learning models understand only numbers but not texts, the inputs should be encoded (= converted into a numerical format).

- **input embeddings** - input embeddings are the inputs converted into a numerical format. 
  
  They function as a kind of a dictionary and help the machine learning model to understand the meaning of the words.

- **positional encoding** - positional encodings are added to the input embeddings to make sure that the original words' order is preserved. 

  This is important because unlike former language models, the language models based on transformers, process the input embeddings not one by one, but analyzes all of them at once. The main advantage of it is the fact that it decreases significantly the processing time. On the other hand, though, problems with information related to words' order may occur.

- **encoder** - the encoder processes the input. 
  
  The role of the encoder is to capture the complex contextual relationships between words and their meaning. It does it through the attention mechanism by applying the so-called attention layers (**Nx**)  

- **decoder** - the main task of the decoder is to generate the output in a form that is understandable for humans, for example a sentence translated into another language. 

  Similar to the encoder, the decoder also consists of attention layers (**Nx**). The decoder takes in input from 2 places:
   
   1. **encoded representation** - the data processed previously by the encoder with the information about the context;
   2. **outputs (shifted right)** - the output generated so far by the decoder, for example a part of the translated sentence.  

   Just like in case of the encoder, where inputs need to be converted into a numerical format, also the outputs (shifted right) have to go through the same process so that the model is able to understand them. They are then called **output embeddings**. They also undergo **positional encoding**, which helps the model understand the order of words in a sentence.

- **linear** - after the decoder produces the output, the linear layer performs some mathematical operations on this data using parameters such as weights and biases. It is a bit like assigning a score to each of the elements in the output.

- **softmax** - the softmax is applied to convert these scores into probabilities. In other words, it indicates how probable it is for each word to be present in the final output.

- **output probabilities** - the final output, for example a sentence translated into another language. 