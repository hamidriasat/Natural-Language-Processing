
### Predicting Hotel Rating from Reviews
Goal was to train a machine learning model that is capable to predict the hotel rating based on the text of the review.


###### Input
Download TripAdvisor Dataset in JSON format (http://times.cs.uiuc.edu/~wang296/Data/). 
In our case we are directly importing the whole dataset into our colab file.

###### EDA
Conduct basic exploratory data analysis (EDA).

#### Technique 
Solved using pretrained [Bert](https://arxiv.org/abs/1810.04805) and [XLnet](https://arxiv.org/abs/1906.08237) for classification Task

### Code Files
* Hotel_Reviews_XLnet_Deployment.ipynb  ==>	Code for deployment of finetuned Xlnet.
* Hotel_Reviews_XLnet_Finetune.ipynb ==>	Finetuning XLnet for classification task.
* Hotel_Riviews_Bert.ipynb  ==> Using bert embeddings to train Logistic Regression and SVM.

```
Dependies:
Python 3.6 or higher
PyTorch 1.2.0 or higher
Transformers v3.1.0
```
