# Explainable-Detection-of-Online-Sexism-EDOS- || Colab: https://colab.research.google.com/drive/1sh2D-NjfLrO_QqGVl556Dd74mVaU96r8?usp=sharing 
###### Competition Project  https://codalab.lisn.upsaclay.fr/competitions/7124 
##### https://github.com/rewire-online/edos

### Used dataset: https://drive.google.com/file/d/1CEPXTzO_cBPiBWQofnyAjmolAUlLIB-N/view 
Sexism is a growing problem online. It can inflict harm on women who are targeted, make online
spaces inaccessible and unwelcoming, and perpetuate social asymmetries and injustices.
Automated tools are now widely deployed to find, and assess sexist content at scale but most
only give classifications for generic, high-level categories, with no further explanation. Flagging
what is sexist content and also explaining why it is sexist improves interpretability, trust and
understanding of the decisions that automated tools use, empowering both users and
moderators.
This task supports the development of English-language models for sexism detection that are
more accurate as well as explainable, with fine-grained classifications for sexist content from
Gab and Reddit.

#### The task contains three hierarchical subtasks:
##### TASK A - Binary Sexism Detection: a two-class (or binary) classification where systems have to
predict whether a post is sexist or not sexist.
##### TASK B - Category of Sexism: for posts which are sexist, a four-class classification where
systems have to predict one of four categories: (1) threats, (2) derogation, (3) animosity, (4)
prejudiced discussions.
##### TASK C - Fine-grained Vector of Sexism: for posts which are sexist, an 11-class classification
where systems have to predict one of 11 fine-grained


# Project Details: 

### Dataset: For this assignment the dataset named, train_all_tasks.csv has been used. 

### Data Loading and Exploration: 

Used several libraries to load the dataset, data cleaning and Perform EDA, as well as for text vectorization as part of the text preprocessing before training the model.

For the data cleaning part, it is checked if there are any null values or any nan values to drop. After that, I have worked on the text preprocessing part, checked the Regular Expressions, Capitalization, double spaces and stopwords to be removed from the dataset and made all the words as lowercase ones. Here to perform the tasks NLTK library has been used here. 

In the EDA part, I looked up statistical analysis here, for example, analyzed the class distributions and analyzed the common words that have been used most frequently in two categories, sexist and non sexist words. Therefore, I analyzed the average length of the texts. 

Other than that, several visualizations has been performed using several python libraries such  as pandas, numpy and matplotlib etc. 

### MODELs Selection and Implementation: 

For task A, I have applied some classification models such as Random Forest and SVM. Before that followed the text vectorization technique of NLP named TFIDF vectorization. Then for task B and task C, a neural network based model has worked properly with better accuracies. The different models' accuracies are for Random forest, SVM and LSTM such as 82%, 67% and 92% accordingly. Therefore, all the model results have been represented with classification reports and Confusion matrix. 

The reason behind why I used all these models, these are quite familiar models that are being used for text classifications, the traditional models and the neural network based models and performs better in terms of showing better performance as a parameter of accuracy. 



