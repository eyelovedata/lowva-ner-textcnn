

# Files

### Pre-processing Data

```CLAMP_postprocessing.ipynb```: Post-processing from CLAMP outputs by 1) cleaning the data, 2) processing the different section headings, 3) formatting it for input into our models.

```lowva-hyperparameterTuning.ipynb```: Hyperparameter tuning on multiple models, and values, including the number of units for the dense layer, the dropout rate for the dropout layers, and the optimal learning rate. We explored multiple models including A) Structured model; B) CNN word embedding text model; C) CUI One-hot text model; D) CUI cui2vec text model; E) Structured and CNN word embedding combined model; F) Structured and CUI one-hot combined model; G) Structured and CUI cui2vec combined model; H) Structured and cui2vec text model and fully connected word embedding model. 

```lowva-finalModels.ipynb```: Using the hyperparameters tuned from before, this trains the models on our testing and validation sets. 

```lowva-finalTest.ipynb```: Using the models trained before, this runs the model with the test set and extracts relevant analyses values. We determined the F1 score by iterating through 0.05 increments of thresholds to arrive at the highest F1 scores for the model. 
