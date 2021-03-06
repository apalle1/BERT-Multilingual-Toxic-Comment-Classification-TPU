# BERT-Multilingual-Toxic-Comment-Classification

# Description

It only takes one toxic comment to sour an online discussion. The Conversation AI team, a research initiative founded by Jigsaw and Google, builds technology to protect voices in conversation. A main area of focus is machine learning models that can identify toxicity in online conversations, where toxicity is defined as anything rude, disrespectful or otherwise likely to make someone leave a discussion. If these toxic contributions can be identified, we could have a safer, more collaborative internet.

In the previous 2018 Toxic Comment Classification Challenge, Kagglers built multi-headed models to recognize toxicity and several subtypes of toxicity. In 2019, in the Unintended Bias in Toxicity Classification Challenge, you worked to build toxicity models that operate fairly across a diverse range of conversations. This year, we're taking advantage of Kaggle's new TPU support and challenging you to build multilingual models with English-only training data.

Jigsaw's API, Perspective, serves toxicity models and others in a growing set of languages (see our documentation for the full list). Over the past year, the field has seen impressive multilingual capabilities from the latest model innovations, including few- and zero-shot learning. We're excited to learn whether these results "translate" (pun intended!) to toxicity classification. Your training data will be the English data provided for our previous two competitions and your test data will be Wikipedia talk page comments in several different languages.

As our computing resources and modeling capabilities grow, so does our potential to support healthy conversations across the globe. Develop strategies to build effective multilingual models and you'll help Conversation AI and the entire industry realize that potential.

# Evaluation

Submissions are evaluated on area under the ROC curve between the predicted probability and the observed target.

# Models

**Multilingual models** 

bert-base-multilingual-uncased - https://huggingface.co/bert-base-multilingual-uncased <br />
XLM-R - https://huggingface.co/xlm-roberta-base

**Monolingual models** 

Spanish - https://huggingface.co/dccuchile/bert-base-spanish-wwm-uncased <br />
Turkish - https://huggingface.co/dbmdz/bert-base-turkish-cased <br />
Russian - https://huggingface.co/DeepPavlov/rubert-base-cased <br />
Portugese - https://huggingface.co/neuralmind/bert-base-portuguese-cased <br />
Italian - https://huggingface.co/dbmdz/bert-base-italian-cased <br />
French - https://huggingface.co/camembert-base

**Using ```translators``` library with Google API, the current training dataset can be translated into Portugal, Turkish, Russian, Italy, Espanol and France languages. Monolingual models are then fine-tuned on translated data.**  


