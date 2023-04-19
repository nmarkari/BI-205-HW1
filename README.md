# BI-205-HW1

This project uses sklearn's LogisticRegression classifier with the "balanced" parameter (weighting classes based on inverse of their proportion of the data).

The model is saved to: "model.sav"

To use model, use the following function:

preprocess_and_predict(X,Y,model_file):

....inputs: 

....X (matrix of shape (1,2048,2048,51) or (2048,2048,51)  last dimension corresponds to channels
    
....Y (matrix of shape (1,2048,2048,2) or (2048,2048,2) where 0/1 are nuclear/whole cell instance segmentation
            model_file
....outputs: y_pred (dictionary of cell_instance:predicted class as a number)
    

Running main_notebook.ipynb downloads the data, preprocesses it, generates "preprocessed_data.csv", makes and saves the correlation heatmap, trains the logistic regression classifier, makes and saves the confusion matrix, and saves the model parameters. "full_data.csv" is the full data from all 40 images, named separately to prevent it from being overwritten when testing out main_notebook.ipynb.  
