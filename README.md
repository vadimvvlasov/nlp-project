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




## Here are some things I looked at while making project:
#### 1) Attention is All You Need 
https://github.com/bentrevett/pytorch-seq2seq/blob/master/6%20-%20Attention%20is%20All%20You%20Need.ipynb

#### 2) Attention Seq2Seq with PyTorch: learning to invert a sequence 
https://towardsdatascience.com/attention-seq2seq-with-pytorch-learning-to-invert-a-sequence-34faf4133e53

#### 3) The Annotated Encoder Decoder 
https://bastings.github.io/annotated_encoder_decoder/

#### 4) Implementing Attention Models in PyTorch 
https://medium.com/intel-student-ambassadors/implementing-attention-models-in-pytorch-f947034b3e66


#### 5) NLP-progress
Repository to track the progress in Natural Language Processing (NLP), including the datasets and the current state-of-the-art for the most common NLP tasks.

http://nlpprogress.com/english/summarization.html

#### 6) The Best NLP Tools of Early 2020: Live Demos
https://towardsdatascience.com/the-best-nlp-tools-of-early-2020-live-demos-b6f507b17b0a

#### 7) NLP FROM SCRATCH: TRANSLATION WITH A SEQUENCE TO SEQUENCE NETWORK AND ATTENTION
https://pytorch.org/tutorials/intermediate/seq2seq_translation_tutorial.html