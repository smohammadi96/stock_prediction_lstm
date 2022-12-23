# stock prediction

## dataset sample

![alt text](https://github.com/smohammadi96/stock_prediction_lstm/blob/main/images/stock_dataset.PNG)



## Results

The plot below, shows the actual value of the close price in the training and testing phase and the actual value as specified
The model has been able to predict the Close price well. The red color is the actual value of the test data, the orange color,
The output value of the model and the blue color shows the value of the close price in the training process.


**LSTM**
![alt text](https://github.com/smohammadi96/stock_prediction_lstm/blob/main/images/plot1.PNG)

**GRU**
![alt text](https://github.com/smohammadi96/stock_prediction_lstm/blob/main/images/plot2.PNG)




| First Header  | Layers number | neurons number in each layer | Optimizer | Rmse without scale | Rmse with scale | 
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | 
| GRU (tanh)  | 3 | 128-64-32 | Adam | 43.14 | 0.01 |
| LSTM | 2 | 128-64 | Adam | 57 | 0.02 |
| GRU | 3 | 128-64-32 | Adam | 59.74 | 0.02 |
| LSTM (tanh) | 2 | 128-64 | Adam | 490 | 0.19 |
| LSTM | 2 | 128-32 | Adam | 53.02 | 0.02 |
| GRU | 2 | 128-64 | Adam | 148 | 0.05 |


The best result that has the lowest MSE is related to the 3-layer GRU network with the number of neurons 64, 128 and 32, which have better results than LSTM. GRU and LSTM both use different ways to avoid vanishing gradient problem.
The main difference between GRU and LSTM is that GRU has two gates that are reset and updated, but LSTM has three gates: input, output, and forget This is because GRU is less complicated and more suitable for small datasets. It is worth mentioning which exposes GRU full memory and hidden layers.
