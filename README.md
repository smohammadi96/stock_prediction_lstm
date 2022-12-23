# stock prediction

## dataset sample

![alt text](https://github.com/smohammadi96/stock_prediction_lstm/blob/main/images/stock_dataset.PNG)



## Results

![alt text](https://github.com/smohammadi96/stock_prediction_lstm/blob/main/images/plot1.PNG)

![alt text](https://github.com/smohammadi96/stock_prediction_lstm/blob/main/images/plot2.PNG)

![alt text](https://github.com/smohammadi96/stock_prediction_lstm/blob/main/images/table.PNG)


| First Header  | Layers number | neurons number in each layer | Optimizer | Rmse without scale | Rmse with scale | 
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | 
| GRU (tanh)  | Content Cell  |
| LSTM | 2 | 128-64 | Adam | 57 | 0.02 |
| GRU | 3 | 128-64-32 | Adam | 59.74 | 0.02 |
| LSTM (tanh) | 2 | 128-64 | Adam | 490 | 0.19 |
| LSTM | 2 | 128-32 | Adam | 53.02 | 0.02 |
| GRU | 2 | 128-64 | Adam | 148 | 0.05 |
