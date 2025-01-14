# Binary classification: Is this bottle of wine red or white?
This is the root directory for an example project for the
[MLflow HuggingFace Recipe](https://mlflow.org/docs/latest/recipes.html#huggingface-recipe).
Follow the instructions [here](../README.md) to set up your environment first,
then use this directory to work with any Huggingface models and dataset,
and evaluate its performance,
all out of box!

In this example, we demonstrate how to use MLflow Recipes to build a Shakespear
text generator by fine-tuning
[the distilled BERT language model](https://huggingface.co/distilbert-base-uncased).
and generate the next sensentce.
The example uses Shakespear.

In this [notebook](notebooks/jupyter.ipynb) ([the Databricks version](notebooks/databricks.py)),
we show how to build and evaluate such a Shakespear text generator step by step,
following the best practices of machine learning engineering.
By the end of this example,
you will learn how to use MLflow Recipes to
- Ingest the raw source data from HuggingFace.
- Splits the dataset into training/validation/test.
- Create a transformer with BERT's tokenizer and transform the dataset.
- Fine-tune a model from DistilBERT to generate the next sentence in the Shakespear style.
- Evaluate the trained model, and improve it by iterating through the `transform` and `train` steps.
- Register the model for production inference.

All of these can be done with Jupyter notebook or on the Databricks environment.
Finally, challenge yourself to build a better model. Try the following:
- Use a different data source to fine-tune the model.
- Fine tune the hyperparameters of the model.