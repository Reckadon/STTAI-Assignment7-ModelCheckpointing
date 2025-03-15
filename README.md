# Assignment 7 - Model Checkpointing

Team 25, Members:     



| Name | Roll Number |  
| ------ | ------ |  
| Romit Mohane | 23110279 |  
| Rudra Pratap Singh | 23110281 |  

## Introduction
This assignment aims to learn about text classification tasks for checkpoint creation.

---

### Code in [Notebook](./STTAI_Lab7.ipynb)

---

### Screenshots

> Model architecture.   
![Model architecture.](./arhitecture.png)
 
> Hyperparameters   
__Case 1: BoW__   
![tokens](./hyperparams1.png)    
_Number of max features for vectorizer_   
![batch size and epochs](./hyperparams2.png)   
_Batch size and lr for dataset 1_   
![batchsize and epohcs](./hyperparams3.png)    
_Batch size and lr with previous best model's checkpoint On IMDB (dataset 2)_<br><br>
> __Case 2: BERT__
> <br>
![tokens BERT](./hyperparams4.png)
> <br>
_Batch Size for the tokenizer_
![batch size and epochs](./hyperparams5.png)
![](./hyperparams6.png)
_Batch size and lr for dataset 1_
![batch size and epochs](./hyperparams7.png)
![](./hyperparams8.png)
_Batch size and lr for dataset 2_


> Logged Metrics
__Case 1: BoW__   
![](./metrics1.png)  
_Metrics while training on dataset 1_  
![](./metrics2.png)   
_Metrics while training (using best trained model checkpoint) on dataset 2_<br><br>
__Case 2: BERT__<br>
![](./metrics3.png)
_Metrics while training on dataset 1_
![](./metrics4.png)
_Metrics while training (using best trained model checkpoint) on dataset 2_


> Confusion matric visualisations  
__Case 1: BoW__  
![](./cfm1.png)  
_Confusion matrix for best model on dataset 1 Validation set_  
![](./cfm2.png)  
_Confusion matrix for best model (from pretrained best checkpoint) on dataset 2 Validation set_<br><br>
__Case 2: BERT__<br>
![](./cfm3.png)<br>
_Confusion matrix for best model on dataset 1 Validation set_
![](./cfm4.png)<br>
_Confusion matrix for best model (from pretrained best checkpoint) on dataset 2 Validation set_  



> Training and validation loss curves.   
__Case 1: BoW__    
![](./curves1.png)    
Curves for training on Dataset 1  
![](./curves3.png)  
Curves for ReSuMe training on Dataset 2 (IMDB)  <br><br>
__Case 2: BERT__<br>
![](./curves5.png)<br>
Curves for training on Dataset 1  
![](./curves6.png)<br>
Curves for ReSuMe training on Dataset 2 (IMDB)  

> Tensorboard comparison
![](./tb1.png)
_Train Loss plot and comparison_
![](./tb2.png)
_Validation Loss plot and comparison_
![](./tb3.png)
_Validition Accuracy plot and comparison_
