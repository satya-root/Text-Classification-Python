# Text-Classification-Python

This repository covers whole range of text classification problems using different machine learning algorithms.

# 1. Installation & Requirements:
The general installation guide to run different projects is provided here. However if any **error** occurs due to missing libraries, please read the error and install the library according to that information.

<p> Clone the tool if you have git installed. </p>
<b> <ul> Git Installation Guide: </b>
  <li>Windows - https://git-scm.com/download/win </li>
  <li>Linux - https://git-scm.com/download/linux </li>
  </ul>
Then run these command in the Command Prompt or Terminal.

```
git clone https://github.com/Yunus0or1/Text-Classification-Python.git
cd Text-Classification-Python
```
<p> <b>        OR </b> </p>
<p> Download from the link: https://github.com/Yunus0or1/Text-Classification-Python/archive/master.zip <p>
Then, run these command in the Command Prompt or Terminal.

```
cd Text-Classification-Python
```

```
pip install -r requirements.txt
```
> There are issues regarding the installation of Tensorflow. To check versioning and other aspects, please click this [link](https://github.com/Yunus0or1/Object-Detection-Python/blob/master/README.md) to make a clear understanding of tensoflow installation guide. 

# Run
These are all **Python** files. 

```
Install Python3 or Python2.7 
Open CMD
Go to directory path and write below command
python3 <filename.py>
```




# 2. Usage:
<p> i. Run the python file from the directories. </p>

<p> Or type the command in terminal/command prompt: </p>

```
python _filename_
```
___

> Source code explanations

___

There is a urge necessity to use **Embedding Layer** in neural network to do text classification. To understand why, hit this [Medium](https://towardsdatascience.com/deep-learning-4-embedding-layers-f9a02d55ac12) article. 
- Convolutional Neural Network in action to do text classification.

 - Layers: Embedding&#8594;Conv1D&#8594;MaxPooling1D&#8594;Conv1D&#8594;MaxPooling1D&#8594;LSTM&#8594;Dense

 - ***softmax*** activatation is used to do a normalized probability distribution among multiple classes.



## NER-Python

 - An NER system using preposition to extract location from social media posts.
 - Uses NLTK library to get the **Parts of Speech** tags and identify place names on three steps.
 - All the POS tags along with a video tutorial can be found in this [link](https://pythonprogramming.net/natural-language-toolkit-nltk-part-speech-tagging/).
 - The program analyses the given String and look up different prepositions in order to find a valid location name


## Neural_Network_Classification

 - ***neural_network_conv.py*** contains source code on **Convolutional Neural Network** in action to do text classification. Layers: Embedding &#8594; Conv1D &#8594; MaxPooling1D &#8594; Conv1D &#8594; MaxPooling1D &#8594; LSTM &#8594; Dense.
 - ***neural_network_dense.py*** contains source code on a very **simple** neural network in action to do text classification. Layers: Dense 256 neurons &#8594; Dense 10 neurons. Very fast to do text classification. No batch.
  - ***neural_network_lstm.py*** contains source code on a **LSTM** neural network in action to do text classification. Layers: Embedding &#8594; Dense &#8594; LSTM &#8594;  Dense.
 - ***softmax*** activatation is used in the last layer to do a normalized probability distribution among multiple classes.
 - Data Labels
 
   ```
   1- Traffic Jam
   2- No Traffic Jam
   3- Road Condition
   6- Accident
   7- Fire
   ````
 
## Neural_Translator

 - A neural network to translate phonetic Bangla to Bangla.
 - For a simple neural tranlator the layer is: GRU &#8594; TimeDistributed &#8594; Dropout &#8594; TimeDistributed .
 - For a complex neural tranlator the layer is: Bidirectional &#8594; TimeDistributed &#8594; Dropout &#8594; TimeDistributed .
 - No hot encoding.
 - However achieved very poor performance due to lack of translation data. Only 400 data are available.
  
## Road-Condition-Analysis

 - This is research based project. The research paper is submitted to **IEEE ICCIT 2020**.
 - The research is based on road condition analyses of Dhaka city from social media posts.
 - ***machine_classification.py***  contains source code of road condition anaylsis using different machine learning algorthims such as **MultinomialNB**, **LogisticRegression**, **KNeighborsClassifier**
  - ***nueraul_classification.py***  contains source code of road condition anaylsis using neural network. This procedure is similar to ***Neural_Network_classification*** problems.
  
  
## Wrong_Word_Correction

 - This is research based project that has been published. Hit this [Journal](http://www.ijcaonline.org/archives/volume176/number27/31370-2020920288 ) to get details on this project.
 - ***wg.py*** contains source code that generates about 80 wrong words from one single **defined** correct word.
 - ***ml.py*** contains source code that classifies wrong words using different machine learning algorthims such as **MultinomialNB**, **LogisticRegression**, **KNeighborsClassifier**, **RandomForestClassifier** etc.
 - To be noted, when running the ***ml.py*** program, it prompts for choices. Theses are the meaning.
 
   ```
   WBT  = Word Based Tokenization
   CBT  = Character Based Tokenization
   ACB = Advance Character Based Tokenization
   
   NON Saved Model processing = Ground up training, evaluation and predict new wrong word
   Saved Model processing = Loading pre trained model weights and predict new wrong word
   ```

