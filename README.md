# Fine-Tune-a-ChatBot

## OBJECTIVE: 
### FINE-TUNE LLM ChatBot to enable it to answer the TECH INTERVIEW questions


## EXAMPLE:
#### Question: "Define nearest neighbour algorithm..."
#### Answer Not Fine-Tuned: "I'm not sure what that means, but I'm sure it's a good thing.""
#### Answer Fine-Tuned: "The nearest neighbour algorithm was one of the first algorithms used to determine a solution to the travelling salesman problem."
####   - The Fine-Tuned answer is much better, revealing the model has learnt from the new data
####   - But the Fine-Tuned answer is not a very extensive since the training data is rather "shallow". 
####   - Basing training data on WIKIPEDIA would definatively improve the "RICHNESS" of the answers.


## ANALYSIS PARAMETERS
### BASED ON: https://blog.gopenai.com/fine-tuning-dialogpt-medium-on-daily-dialog-dataset-a-step-by-step-guide-4eaecc1b9323
### Train Data: https://drive.google.com/file/d/1WPY3HB3BlXD-Pflk-CbN60_rTQ8eMNlt/view
### LLM Model: DialoGPT-Medium @ HuggingFace
### Train: Colab T4 Instance


## INPUT DATA OVERVIEW
### Example modifies input to a single string 
### But additional attributes in the dataset are structured as lists
### with as many elements as there are iterations of the conversation...
### Thus we have structured the dialogs as list with 
### as many sting entries as the number of iterations of the conversation (here only 2: Q:, A:)
