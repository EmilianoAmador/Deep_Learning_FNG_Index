# Neurotic Fear and Greed Index to Predict Closing Prices
<p align="center">
  <img src="https://github.com/EmilianoAmador/Deep_Learning_FNG_Index/blob/master/Images/FNG-Image.jpg" />
</p>
<br/>
This activity reviews a Recurrent Neural Network (RNN) model's ability to predict Bitcoin closing prices using Fear and Greed Index historic data. More specifically, this activity focuses on Long-Short Term Memory (LSTM) model, a type of RNN with a mathematical backbone perfect for recognizing patterns in sequence of numerical data, to compare its predictive ability when trained with FNG historical data versus when it's trained with closing price historical data. Then its performance is reviewed to illustrate which data is more valuable when predicting future results.


### Fear and Greed Index LSTM Model
![](Images/FNGloss.png)
<br/>
![](Images/FNGParam.png)
<br/>
![](Images/FNGtable.png)
<br/>
![](Images/FNGat5.png)


### Closing Prices LSTM Model
![](Images/CLSloss.png)
<br/>
![](Images/CLSparam.png)
<br/>
![](Images/CLStable.png)
<br/>
![](Images/CLSat5.png)

### Conclusion

The training model with closing prices has a lower loss number of 0.015, while the one training with FNG index has a loss function of 0.13. This means that the training model with the closing prices made less errors after each iteration of optimization. Therefore, this model can track the actual values better than the FNG model. The FNG model does not come near to th epredicting power of the other model.

One detail I noticed was that the models performed best with a window size of 1. The higher the window the worst the performance. As far as the unit number features, the model demonstrated opposing performance. the FNG performs better with a unit numbers of 30, while the closing price model performs better with a unit number of 5. All in all, more research must be done before using these models in an investment firm.
