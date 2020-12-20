# xgboost_with_model_explanation
Demonstration of xgboost model explanation using shapley values on UCI census dataset \
Step-1: Train the classifier (`train_xgb_model.ipynb`)  
Step-2: Explain the model using tree explainer (`xgb_model_explanation.ipynb`)  
Step-3: Convert the trained model to ONNX format using `onnx/onnx-ecosystem` container (`convert_xgb_model_2_onnx.ipynb`)  
Step-4: Load ONNX model to perform test inference (`load_onnx_model.ipynb`)  

Notes: The python packages (ex:`xgboost`) used in the container image `onnx/onnx-ecosystem` are not the latest versions. The Step-3 notebook works fine in the container (which uses an old xgboost version ),but reports an error  with the newer `xgboost` version (say,1.3). 
Also, the container image with old `xgboost` version has difficulty to load the model trained elsewhere with newer `xgboost` version .  




