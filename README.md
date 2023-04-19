# BI-205-HW1

model is saved to: "model.sav"

To use model, use the following function:

preprocess_and_predict(X,Y,model_file):

....inputs: 

....X (matrix of shape (1,2048,2048,51) or (2048,2048,51)  last dimension corresponds to channels
    
....Y (matrix of shape (1,2048,2048,2) or (2048,2048,2) where 0/1 are nuclear/whole cell instance segmentation
            model_file
....outputs: y_pred (dictionary of cell_instance:predicted class as a number)
    
