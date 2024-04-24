# Shallow Learning for long-term Cyanobacterial Bloom forecasting

Code for the project "Shallow Learning for long-term Cyanobacterial Bloom forecasting".

## Dataset

Due to copyright reasons the dataset used for training and testing the network can not be open sourced. We encourage the use of your own data to test the proposed model and code. The current code expect a .xlsx file with the following categories:

```
date: date information for each sample
D: Depth information
T: Temperature value
DO: Dissolved Oxygen
PH: PH value
FC_IVF: phycocianin value
``` 

Feel free to change the code to adapt to your own nomenclature or to add/remove parameters.

## Model
The `models/model.h5` contains the weight of the model used for the results presented in the paper. The code presented allow the train of new models using the `TRAIN` flag.


```
TRAIN = 0: Loads the selected model defined within "model = load_model('../models/model.h5')"

TRAIN = 1: Trains a new model using the same architecture as proposed in the paper.
``` 

The already trained model is suggested as a baseline. We recommend training new models when neeeded.

## How to use

All the code is defined within the `src/LSTM-bloom-prediction.ipynb` Jupyter Notebook. 





