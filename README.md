# machine_translation

## Abstract

Machine translation is a central task in natural language processing. It aims to translate text between languages to overcome communication barriers. Traditional machine translation methods, such as phrase-based or rule-based models, often fall short in handling language complexities ranging from idiomatic expressions to syntactic nuances. Machine translation with deep learning, especially with sequence-to-sequence (seq2seq) model, has achieved substantial improvements in translation performance due to its ability to capture and learn complex language mappings [1].

This project focuses on understanding how dataset characteristics affect machine translation performance. Specifically, we will compare the impact of formal, structured datasets versus informal, conversational ones. We will use French-to-English translation as our test case, given the availability of large, freely accessible datasets that fit these criteria. Our goal is to analyze how current machine translation models respond to diverse linguistic styles.

To achieve this, we will train and test the same model on each dataset type separately, and then evaluate how the model performs when applied across dataset types. By testing each model on examples from both datasets, we aim to determine which dataset type better supports generalization in machine translation.

Understanding which types of data best support generalization will inform the development of future machine translation models. Rather than focusing solely on model advancements, we can improve machine translation performance by building datasets tailored to enhance model training outcomes and foster more effective and adaptable translation systems.

## Directory Organization

machine_translation<br />
|- models<br />
|&emsp;|- tatoeba<br />
|&emsp;│&emsp;|- mt_tatoeba.pt<br />
|&emsp;|- wiki<br />
|&emsp;│&emsp;|- mt_wiki.pt<br />
|- notebooks<br />
|&emsp;|- mt_tatoeba-torchtext.ipynb<br />
|&emsp;|- mt_wiki-torchtext.ipynb<br />
|- data<br />
|&emsp;|- wiki<br />
|&emsp;│&emsp;|- eng-fra.txt<br />
|&emsp;|- tatoeba<br />
|&emsp;│&emsp;|- eng-fra.txt<br />
|- results<br />
|&emsp;|- tatoeba_results.txt<br />
|&emsp;|- wiki_results.txt<br />
