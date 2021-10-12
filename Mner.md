<img src="https://github.com/iAveshh/Dr.nlp/blob/main/drnlp.jpg"/>




## What is Dr.NLP?

Dr.NLP is a natural language process based NER(Named entity rocgnizer) system, which accepts patient narratives as an input and can generate classification based on the narratives. 

These classifications can be generalized into give classes:
1. Actual Disease
2. Preoprative Disease
3. Drugs
4. Medical Disorders, etc.

## Learn more about label studio here - [Website](https://labelstud.io/)

Missing features from Label Studio that has been implemented in this repository are:
1. Spacy 2.0 NER (Named entity Recognition)
2. Spacy 2.0 NER and Relations

Below steps demonstrate, how to get the code working: 

Step 1: Install label-studio as per instructions presented here - https://labelstud.io/

Step 2: After installing, navigate to label_studio --> data_export --> models.py 

In the models.py file look for, 
" from label_studio_converter import Converter " line of code. 

The converter module should come from a location outside the project files, normally when working with anaconda the modules comes,

from - " C:\Users\user_name\\.conda\envs\label-studio\Lib\site-packages\label_studio_converter"

Replace the converter file with the file in this repository. 

  DONE! 

Step 3: For, NER annotations import a text file , annotate the file when opted for settings under 'NLP' Select "NER"

Example:

 <img src="https://github.gsissc.myatos.net/a771661/Label-Studio-Spacy-2.0/blob/main/NER%20Example.PNG" align="center" /></a>

Now, after annotations are done simply click on export and save the file.

  <img src="https://github.gsissc.myatos.net/a771661/Label-Studio-Spacy-2.0/blob/main/export%20ner.PNG" align="center" /></a>

  NOTE: Relations cannot be extracted with the above configuration, for relations as well as NER extractions follow below steps:

1. From project setting under "NLP" Select "Relation Extraction" 

  Example:

<img src="https://github.gsissc.myatos.net/a771661/Label-Studio-Spacy-2.0/blob/main/Relations.PNG" align="center" /></a>

Annotate the labels, annd create relations as you will normally do, for Label_studio relations and Export the file, by click on " Spacy 2.0 (Relation Extraction)"

Example:

<img src="https://github.gsissc.myatos.net/a771661/Label-Studio-Spacy-2.0/blob/main/export%20relations.PNG" /></a>

