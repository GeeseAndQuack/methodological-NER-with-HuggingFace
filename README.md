# methodological-NER-with-HuggingFace
Dissertation project fine-tuning BERT models for methodological NER for psychology papers.

There is a different ipynb for each of the BERT model's fine-tuned for the methodological NER. These were, BERT, BioBERT, SciBERT and NER-BERT. Overall, the ipynbs are essentially identical other than the different models selected, having them on different notebooks allowed me to train a few models simultaneously using Google Colab Pro.

The datasets are somewhat irritatingly stored in seperate JSON files as a result of the time constraint I had when completing my dissertation. The datasets were being continually created by myself and an expert on psychology methodologies as I was developing the model and writing the dissertation script.

Two outputs have been suppressed from each ipynb, the output of the PBT algorithm and the cross-validation. 

If you wish to recreate the results you simply need to download each of the JSON files and replace the directories I used for each of the Pandas Dataframes used to import the data into python.

Finally, much of the HuggingFace code was taken from this notebook: ___________________________________________-
