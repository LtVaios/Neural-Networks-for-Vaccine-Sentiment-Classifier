# A.I-Vaccine Sentiment Classifier
In this project I use artificial intelligence and deep neural-networks to train a model to be able to tell if a person is an anti-vax, a pro-vax or none just by giving a tweet of theirs as input. Dataset Cleaning, Model Training, Plotting, statistics and metrics are included. These models should have more than 72% accuracy on a similar testset!

## Installation / Run
🛠️ You can download and open the jupyter notebooks in any platform that supports it, like google collab which is where this classifier was developed. You will also find the datasets in /data/ that the model uses to train and evaluate. Make sure to make a file named "data" in google collab and upload the datasets inside in order to instantly run the code.

## 📝 Dataset
Used a ready-to-go twitter dataset with each tweet marked if it is an anti-vax, pro-vax or a neutral
## 📎 Hyperparameters for feed-forward-NN
### :white_check_mark: Model 1 (Tanh)
    ▶️Activation function: Tanh
    ▶️Layers: 5
    ▶️Size of layers: 256 -> 128 -> 64 -> 32 -> 3(output)
    ▶️Dropout Layers: 30%, 20%
    ▶️Learning Rate: 9e-4
    ▶️Loss Function: Cross Entropy Loss  
    ▶️Optimizer: RAdam
    ▶️Batch size: 400
    ▶️Epochs: 50
    ▶️Also used:  dataset cleaning, Batch normalization, built-in sigmoid function
    
### :white_check_mark: Model 2 (PReLU)
    ▶️Activation function: PReLU
    ▶️Layers: 5
    ▶️Size of layers: 125 -> 125 -> 75 -> 30 -> 3(output)
    ▶️Dropout Layers: 30%, 20%
    ▶️Learning Rate: 2e-4
    ▶️Loss Function: Cross Entropy Loss  
    ▶️Optimizer: RAdam
    ▶️Batch size: 450
    ▶️Epochs: 50
    ▶️Also used:  dataset cleaning, Batch normalization, built-in sigmoid function
  
## 📎 Hyperparameters for BiDirectional Stacked RNN's
### :white_check_mark: Model 1 (LSTM Cell)
    ▶️Layers: 3
    ▶️Number of hidden layers: 50
    ▶️Gradient Cliping Rate: 4 
    ▶️Learning Rate: 8e-4
    ▶️Dropout Propability: 25%
    ▶️Loss Function: Cross Entropy Loss  
    ▶️Optimizer: Adam
    ▶️Batch size: 400
    ▶️Epochs: 5
### :white_check_mark: Model 2 (GRU Cell)
    ▶️Layers: 4
    ▶️Number of hidden layers: 30
    ▶️Gradient Cliping Rate: 4
    ▶️Learning Rate: 1e-3
    ▶️Dropout Propability: 30%
    ▶️Loss Function: Cross Entropy Loss  
    ▶️Optimizer: Adam
    ▶️Batch size: 300
    ▶️Epochs: 5
    
 ## Built With
<p float="left">
<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/110px-Python-logo-notext.svg.png" alt="MarineGEO circle logo" style="height: 100px; width:100px;"/>  
&emsp;&emsp;<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/10/PyTorch_logo_icon.svg/198px-PyTorch_logo_icon.svg.png" alt="MarineGEO circle logo" style="height: 120px; width:100px;"/>   <t />  
&emsp;&emsp;<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/38/Jupyter_logo.svg/207px-Jupyter_logo.svg.png" style="height: 100px; width:100px;"/>
&emsp;&emsp;<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/31/NumPy_logo_2020.svg/320px-NumPy_logo_2020.svg.png" alt="MarineGEO circle logo" style="height: 100px; width:200px;"/>
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d0/Google_Colaboratory_SVG_Logo.svg/320px-Google_Colaboratory_SVG_Logo.svg.png" alt="MarineGEO circle logo" style="height: 100px; width:170px;"/>

 </p>
