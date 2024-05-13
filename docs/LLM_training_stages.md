---
title: LLM training stages
layout: default
parent: LLM training
nav_order: 1
---

# LLM training stages

<p style= "padding: 35px 5px 5px;">Training of LLM-s is somehow similar to the way children learn how to speak - they start with words, later they can speak in complete sentences. With time, guidance and feedback, the child learns not only how to speak but also to have conversations and interact.</p>

LLM training can be divided into several stages:

1. **data collection & pre-processing** - LLM-s need to be trained on (vast amounts of) data. That is why the first step is to collect data and compile a training dataset. The data used for training is typically web-crawled data from various sources, such as websites, books, articles, and open-source datasets.

   Then, the data needs to be pre-processed, that is cleansed from as much unwanted content as possible. This can involve getting rid of duplications, personal identifiable information and potentially harmful content. The better the data quality, the better for the LLM training because the well-known principle "garbage in = garbage out" applies also here.

2. **model configuration** - LLM-s are based on transformers, that is deep-learning neural networks. Before the training starts, certain parameters have to be set up for the transformer: the model size,  the number of layers, the number of attention heads, or the learning rate.

3. **pre-training** - in this part of the training process, the language model is fed with huge amounts of previously collected and pre-processed data. The task for the model here is to analyze and make sense of it. Since the data is unlabeled, the model learns without explicit guidance. 
   
   Pre-training often utilizes [transformer architecture](https://milenajoanna.github.io/FinalProjectVistulaLLM-sForBeginners/docs/Transformer_architecture.html) with the [attention mechanism](https://milenajoanna.github.io/FinalProjectVistulaLLM-sForBeginners/docs/Attention_mechanism.html) through which the model is trained to predict missing or masked words within sentences. This cycle is repeated many times until the model achieves optimal performance.

4. **fine-tuning** - in this phase, a language model is trained on a smaller, more specific subset of the pre-training labeled data. The goal is to improve the model's abilities for particular tasks or domains. 
   
   Depending on what the language model should be specifically made better for, the fine-tuning can be approached in several ways like:
  
    - **supervised fine-tuning** - the most common fine-tuning approach. The language model is trained on a labeled dataset that is specific to the task that needs refinement, such as named entity recognition or text classification.

   - **few-shot learning** - the model is fine-tuned by providing a few examples (shots) of the task at the beginning of the input prompts. This provides a better context and improves quality without costly iterations.

   - **domain-specific fine-tuning** - the model is fine-tuned for a specific domain or industry. It learns from professional datasets (like legal, medical, or technical texts) to boost its language understanding about this particular field.

   - **adversarial fine-tuning** - the model is fine-tuned with data that is challenging or tricky so that it learns how to handle problematic questions.

5. **evaluation** - using task-specific metrics, such as perplexity for language modeling, F1 score for named entity recognition, and accuracy for text classification tasks.

  
  
 











 

  
 
  




