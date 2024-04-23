---
title: Types of LLM-s
layout: default
nav_order: 4
---

# Types of LLM-s

<p style= "padding: 35px 25px 5px;">Depending on what we take into account as criteria, we can distinguish the following types of large language models: </p>

- **language representation models** - general purpose LLM models that are trained on huge amounts of text. They can be fine-tuned for specific tasks. Examples of such models are:
  1. **GPT-3 (Generative Pre-trained Transformer)** - developed by OpenAI. It's designed to understand and generate human-like text based on the input it receives. GPT-3 has been trained on a vast amount of internet text and can perform various language-related tasks.
   
  2. **BERT (Bidirectional Encoder Representations from Transformers)** - developed by Google. It understands the context of words in a sentence by considering both the words that come before and after each word. This helps it grasp the meaning of a word based on its surrounding words, making it very good at understanding and generating natural language text.
   
  
- **multimodal models** - language models were first built for text, but now there are also multimodal models that can handle not only text but also other media, like images and videos. Examples of such models are:
  1. **CLIP** - developed by OpenAI. It links text to images and images to text. It's works well for tasks like describing images with text and finding images based on text descriptions.
   
  2. **Sora** - developed by OpenAI. Its's an AI model that can create realistic and creative short videos from text instructions. 


- **fine-tuned or domain-specific models** - when it comes to language representation models, they're quite flexible, but they might not always do their best for certain jobs or subjects. That's why they have to be fine-tuned and trained on texts from a specific domain like science, medicine or law. Examples of such models are:
  
  1. **BioBERT** — a variant of BERT language model trained on biomedical literature. It's used for biomedical text mining tasks like named entity recognition and relation extraction in the medical domain.
   
  2. **LegalBERT** - a variant of BERT language model fine-tuned on legal texts such as court opinions, statutes, and regulations. It performs legal NLP tasks such as legal document classification and legal information retrieval.


- **open source models** - language models whose source code is publicly available and can be freely accessed, used, modified, and distributed by anyone. Examples of such models are:
  
  1. **LLaMa 2** - developed by Meta. LLaMA 2 was introduced in July 2023 for research and business purposes. It's a pre-trained text model with 7 to 70 billion parameters. It's fine-tuned using Reinforcement Learning from Human Feedback (RLHF). LLaMA 2 is versatile, serving as a chatbot and adaptable for various text generation tasks, like coding. 
   
  2. **BLOOM** - launched in 2022 after a global collaboration with volunteers from 70+ countries and Hugging Face researchers. It's an autoregressive text model designed to generate text from prompts using huge computational resources. BLOOM can be used for free through the Hugging Face ecosystem.

- **closed source models** - language models developed and maintained by organizations or companies without publicly available source code. They are often commercial products and details of their architecture as well as training data are kept confidential. Examples of such models are:
  
  1. **Google Gemini (formerly Bard)** - an AI chatbot developed by Google. Unlike older Google AI, Gemini is multimodal - it understands various data types like audio, images, and text. This lets it solve complex problems, like understanding handwritten notes or graphs. Gemini can directly handle text, images, audio, and video as mixed data sequences.
   
  2. **Claude 3** - developed by Anthropic. Claude 3 comes in three versions: Haiku, Sonnet, and Opus, each smarter than the last. It's Anthropic's first try at multimodal AI and it's a significant upgrade from previous Claude versions that were known for being overly cautious about AI safety. For example, Claude 2's safety measures were so strict that the chatbot avoided discussing many topics, even ones without obvious safety concerns.









  