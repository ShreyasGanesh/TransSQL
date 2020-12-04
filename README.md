# TransSQL
This is the project repository for the NLP task of converting text to SQL using Transformers.

## Project Structure

1.  Models: This folder contains the models which were used in the experiments. Each Jupyter notebook corresponds to a different model as follows:

    1. `ROBERTA_BERT.ipynb`: The model which uses RoBERTa as the encoder and BERT as the decoder.
    2. `DistilBert.ipynb`: The model which uses DistilBERT as the encoder and BERT as the decoder.
    3. `BART.ipynb`: The model which uses BART as both encoder and the decoder.
    4. `BART_50_Intermediate_Tuned.ipynb`: The model which uses BART as both encoder and the decoder and has intermediate fine tuning done.
    5. Scaled Loss Model to be added.
    
2. Evaluation: This folder contains a single Jupyter notebook - `Evaluation.ipynb`, which is used to evaluate the models.
3. db: This folder contains some db files which are used in the evaluation.

## Dataset
We used the WikiSQL dataset for training, which can be found here: https://github.com/salesforce/WikiSQL.
