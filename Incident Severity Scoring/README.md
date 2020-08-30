# Incident Severity Scoring

## [Bert](https://arxiv.org/abs/1810.04805) and [XLnet](https://arxiv.org/abs/1906.08237) for classification Task

The goal was to estimate incident severity from given articles. It was open ended problem so different approaches were tested like Rule based classification, training Logistic Regression and SVM, fine tuning BERT and XLNET. After performing upsampling and
summarizing articles with BERT extractive summarizer, fine-tuned XLNET model was selected because of best results. This project was implemented in PyTorch with pre-trained “xlnet-base-cased” model provided by Hugging Face library.


### Code Files
* Incident_Project_Bert.ipynb ==>	Using bert embeddings to train 	Logistic Regression and SVM.
* Incident_Project_Bert_Finetune.ipynb ==>	Finetuning bert for classification task
* Incident_Project_Oversampling_XLnet_Finetune.ipynb ==>	Finetuning XLnet after performing upsampling on data.
* Incident_Project_XLnet_Deployment.ipynb ==>	Code for deployment of finetuned Xlnet.
* Incident_Project_XLnet_Finetune.ipynb ==>		Finetuning XLnet for classification task
* Incident_Project_XLnet_with_summerizer_Finetune.ipynb ==>	First summerize articles with pretrained bert then finetune Xlnet
on summerized articles.

```
Dependies:
Python 3
Pytorch
```
