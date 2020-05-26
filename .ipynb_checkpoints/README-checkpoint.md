# nlp-project
# Headlines generation from news articles in Russian

## Description
With the rapid spread of online news, users can be overwhelmed with huge amounts of information. Understandind all of this data is time consuming. So summarizing can help us to process and understand these data. On the other hand headlines are becoming increasingly important to attract readers to news articles.

News headline generation is a subtask of summarization which has been extensively studied recently.
Seq2Seq is the most common model for generating text for various languages. At the same time, the use of Seq2Seq for texts in Russian is currently poorly understood.

In this project I'm going to train a neural network to generate headlines with the "Rossiya Segodnya" news dataset.

## idea
I'm going to make Data preprocessing and then use Pre-trained embeddings to build sequence to sequence network with  attention mechanism in pyTorch implementation.

## Dataset
https://github.com/RossiyaSegodnya/ria_news_dataset
##  Evaluation Metrics 
ROUGE-1, ROUGE-2, ROUGE-L
## Tools
- PyTorch
- PyRouge for ROUGE Score Evaluation
- 

## Approach
- Preprocessing
 - Clearing
 - Tokenization
 - Use pretrained word embedding
 - Vectorization
- Designing GRU Bi-directional Encoder-Decoder layers with attention mechanism
- Train model
- Take user input and use model to generate headline


## References
1. Daniil Gavrilov, Pavel Kalaidin, and Valentin Malykh. Self-Attentive Model for Headline Generation. 41st European Conference on Information Retrieval, 2019. arXiv:1901.07786 [ arXiv:1901.07786 [cs.CL]](https://arxiv.org/abs/1901.07786)
2. Claudio Mastronardo, Fabio Tamburini. Enhancing a Text Summarization System with ELMo [PDF](https://pdfs.semanticscholar.org/bb1b/e9c9338291ef198c03f46ff19a68094f995d.pdf)
3. Tao Luo, Kun Guo, Hong Guo. Automatic Text Summarization Based on Transformer and Switchable Normalization.
