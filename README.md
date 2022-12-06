# methodological-NER-with-HuggingFace
Dissertation project fine-tuning BERT models for methodological NER in pscyhology papers.

There is a different ipynb for each of the BERT model's fine-tuned for the methodological NER. These were, BERT, BioBERT, SciBERT and NER-BERT. Overall, the ipynbs are essentially identical other than the different models selected, having them on different notebooks allowed me to train a few models simultaneously using Google Colab Pro.

The datasets are somewhat irritatingly stored in seperate JSON files as a result of the time constraint I had when completing my dissertation. The datasets were being continually created by myself and an expert on psychology methodologies as I was developing the model and writing the dissertation script.

A few of the outputs have been suppressed from the notebooks as they signigicantly cluttered the output. The output of the installation of the libraries at the start was suppressed as well as the output of the population based training algorithm and the cross-validation.

If you wish to recreate the results you simply need to download each of the JSON files and replace the directories I used for each of the Pandas Dataframes used to import the data into python.

Finally, the following notebook was a significant help in terms of setting up the fine-tuning process of which the compute metrics and tokenize and align label functions have been completely ripped from: ___________________________________________-

Overall my view on the model performance is that much work is still needed to be done to achieve the results I would desire. Much of these improvements were clearly laid out in my dissertation but have yet to be implemented. Performance across the models in the final implementation ended up being fairly similar with the highest performing model being BioBERT with an average F1-score across all entity groups of 0.678. The final implementation sought to avoid some of the likely overfitting that was occurring through the PBT algorithm so the highest peforming hyperparameters were taken and applied to a freshly generated train-test split of the dataset.

If you would like to have a gander at the full script of my dissertation for any reason, just contact me.
