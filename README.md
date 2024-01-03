# pubmed_literature_scan

This project aims to replicate the state-of-the-art neural network model presented in the paper "Neural Networks for Joint Sentence Classification in Medical Paper Abstracts." 

The original paper addresses the challenge of efficiently classifying sentences in unstructured medical abstracts, providing a valuable tool for information extraction. Model 5 incorporates additional improvements to capture the relative positions of sentences in the abstracts.

# Metrics
| Model Architecture                                                               | accuracy | precision | recall | f1    |
|----------------------------------------------------------------------------------|----------|-----------|--------|-------|
| Baseline (TF-IDF Multinomial Naive Bayes Classifier)                             | 72.18    | 0.718     | 0.721  | 0.698 |
| Conv1D                                                                           | 78.34    | 0.779     | 0.783  | 0.780 |
| Univeral Sentence Encoder                                                        | 69.78    | 0.697     | 0.697 | 0.694 |
| Conv1D + Character Level Embeddings                                              | 66.16    | 0.652     | 0.661  | 0.651 |
| Pretrained Token Embeddings + Character Level Embeddings                         | 69.22    | 0.707     | 0.692  | 0.689 |
| Pretrained Token Embeddings + Character Level Embeddings + Positional Embeddings (10% data) | 78.65    | 0.798     | 0.786  | 0.783 |

### Model 6 architecture
![model](https://github.com/smellycloud/pubmed_literature_scan/assets/52908667/f08f64b7-4c7e-4bc7-8f48-d6dcae25287e)

### Model 5 architecture
![model4](https://github.com/smellycloud/pubmed_literature_scan/assets/52908667/5695541d-2dfc-404a-8ad2-c38603227cfe)


