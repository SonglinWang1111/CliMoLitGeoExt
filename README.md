# CliMoLitGeoExt
## Introduction
The brief idea of this program is to investigate the usability of LLMs in geographic knowledge extraction and text classification, with PopGeo (Climate Mobility) literature as a case study. Its goals are two fold - on the one hand, to evaluate the performance of current GenAI models on domain specific tasks, their consistancy in cognition, their brittleness, and their statistically correctness and so on and so forth; and on the other hand, to enhance the common existing, time-consuming manual workflow in text classification in human or population geography fields. The evaluation was conducted among diverse models, temperatures, and prompting approaches, plus comparisons among GenAI, discriminative AI (BERTopic), traditional NLP (LDA). Currently, please find the program in branch 'master'.

## Content
### Data
All 30 papers used for testing the text classification performance are saved in folder 'data'.
### Examples
All 3 papers as input of the few-shot prompting are saved in folder called 'examples'.
### Parsing
The 'pdf2text' script uses another tool for parsing PDF literature in 'data' and 'example' folders as Python Dictionaries respectively. The way to access that tool as well as reference are in this script. Since some LLMs does not accept PDF as input, we currently use another tool to parse them in advance, for a better comparison. The results are then saved as the .npy files respectively. 
### Initial experiments: Python scripts starting with 'prompt', excel document 'manual', csv documents and folder 'plots'
In experiment 'together', I ask LLMs to response all metrics together, based on one testing paper, either as a Python Dictionary or as a Python List, then conducted evaluation with the manual classification result. For the experimant 'separate', I ask LLMs to response subsets of metrics. Please note that you have to put your own APIs in a .txt folder in correct order. The classification results are saved as correspnding .csv documents, while the evaluation results are saved in 'plots' folder. 
### Experiment on all 30 papers
Currently this is not committed.
### Baseline
I use LDA and BERTopic as baseline models for comparisons. Please find the corresponding Python scripts.
