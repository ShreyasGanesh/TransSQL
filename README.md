# TransSQL
This is the project repository for the NLP task of converting text to SQL using Transformers.

## Project Structure

1.  Models: This folder contains the models which were used in the experiments. Each Jupyter notebook corresponds to a different model as follows:

    1. `ROBERTA_BERT.ipynb`: The model which uses RoBERTa as the encoder and BERT as the decoder.
    2. `DistilBert.ipynb`: The model which uses DistilBERT as the encoder and BERT as the decoder.
    3. `BART.ipynb`: The model which uses BART as both encoder and the decoder.
    4. `BART_50_Intermediate_Tuned.ipynb`: The model which uses BART as both encoder and the decoder and has intermediate fine tuning done.
    5. `BART_Scaled_Evaluation.ipynb`: The model which uses BART as both encoder and the decoder and a scaled loss function.
    
2. Evaluation: This folder contains a single Jupyter notebook - `Evaluation.ipynb`, which is used to evaluate the models.
3. db: This folder contains some db files which are used in the evaluation.
4. Errors:
    1. `errors.txt` which contains all the queries from the test set where our best model (BART with intermediate fine tuning) failed. 
    2. `Error Analysis.xlsx` which contains 100 manually annotated examples of failed queried and why they failed.

## Dataset

We used the WikiSQL dataset for training, which can be found here: https://github.com/salesforce/WikiSQL. Additionally, we are using the Spider dataset (https://yale-lily.github.io//spider) for intermediate fine tuning of our models.

## Baseline Model

The implementation of the baseline model which we are using (https://arxiv.org/pdf/1709.00103.pdf), can be found here - https://github.com/tiwarikajal/Seq2SQL--Natural-Language-sentences-to-SQL-Queries
