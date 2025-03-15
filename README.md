# Assignment 7 - Model Checkpointing

Team 25, Members:

| Name               | Roll Number |
| ------------------ | ----------- |
| Romit Mohane       | 23110279    |
| Rudra Pratap Singh | 23110281    |

## Introduction

This assignment aims to learn about text classification tasks for checkpoint creation.

---

### Code in [Notebook](./STTAI_Lab7.ipynb)

---

### Screenshots

> Model architecture.  
> ![Model architecture.](./arhitecture.png)

> Hyperparameters  
> **Case 1: BoW**  
> ![tokens](./hyperparams1.png)  
> _Number of max features for vectorizer_  
> ![batch size and epochs](./hyperparams2.png)  
> _Batch size and lr for dataset 1_  
> ![batchsize and epohcs](./hyperparams3.png)  
> _Batch size and lr with previous best model's checkpoint On IMDB (dataset 2)_<br><br> > **Case 2: BERT**  
> ![tokens BERT](./hyperparams4.png)  
> _Batch Size for the tokenizer_  
> ![batch size and epochs](./hyperparams5.png)
> ![](./hyperparams6.png)
> _Batch size and lr for dataset 1_
> ![batch size and epochs](./hyperparams7.png)
> ![](./hyperparams8.png)
> _Batch size and lr for dataset 2_

> Logged Metrics
> **Case 1: BoW**  
> ![](./metrics1.png)  
> _Metrics while training on dataset 1_  
> ![](./metrics2.png)  
> _Metrics while training (using best trained model checkpoint) on dataset 2_<br>
> **Case 2: BERT** <br>
> ![](./metrics3.png)<br>
> _Metrics while training on dataset 1_<br>   
> ![](./metrics4.png)<br>   
> _Metrics while training (using best trained model checkpoint) on dataset 2_   

> Confusion matric visualisations  
> **Case 1: BoW**  
> ![](./cfm1.png)  
> _Confusion matrix for best model on dataset 1 Validation set_  
> ![](./cfm2.png)  
> _Confusion matrix for best model (from pretrained best checkpoint) on dataset 2 Validation set_<br><br>
> **Case 2: BERT** <br>
> ![](./cfm3.png)<br>
> _Confusion matrix for best model on dataset 1 Validation set_
> ![](./cfm4.png)<br>
> _Confusion matrix for best model (from pretrained best checkpoint) on dataset 2 Validation set_

> Training and validation loss curves.  
> **Case 1: BoW**  
> ![](./curves1.png)  
> Curves for training on Dataset 1  
> ![](./curves3.png)  
> Curves for ReSuMe training on Dataset 2 (IMDB) <br><br>
> **Case 2: BERT** <br>
> ![](./curves5.png)<br>
> Curves for training on Dataset 1  
> ![](./curves6.png)<br>
> Curves for ReSuMe training on Dataset 2 (IMDB)

> Tensorboard Integration (Final Evaluation)  
![](./tbIntegration.png)   
_You can see the tensorboard integration of the models metrics on colab_   
> ![](./tb1.png)   
> _Train Loss plot and comparison_   
> ![](./tb2.png)   
> _Validation Loss plot and comparison_   
> ![](./tb3.png)   
> _Validition Accuracy plot and comparison_   

**Final Validation Accuracies**

| Method          | Dataset 1 | Dataset 2 |
| --------------- | --------- | --------- |
| BoW             | ~80%      | ~89%      |
| BERT Embeddings | ~87%      | ~87.5%    |

> Checkpoint Compression  
> ![](./compression.png)  
> _Here you can see we are saving the checkpoint as a compressed zip file, and then reading from it as well._
