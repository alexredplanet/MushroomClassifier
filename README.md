This is an old project from 2020 on predicting 1000 mushroom species from image data. 

The data was kindly provided by mushroomobserver.org. 

I am revisiting this as the dataset is highly interesting as a playground to test ideas. 
This is because the data contains:
- highly noisy labels (labels are from a user voting system)
- feature noise (images are uploaded by individual users)
- highly imbalanced classes

The current version of the project uses simple deep learning models (ResNet variants) and the FastAI library. 
One interesting idea I toyed with here was a hierarchical model, where a genus level classifier was first trained, 
and then for each genus, a species level classifier was trained. I tried this as it would allow for new mushroom species to be gradually added to the model over time, with much faster retraining than a single species level model.

I haven't uploaded the model files as they are very large, nor have I uploaded the image files. The notebooks will download all relevant data and generate all models. 