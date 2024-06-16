This is a mini project of Deep learning and Neural network course.
In this miniproject i have used MLP regressor and SVR model for shallow and in deep learning model, 
i have used LSTM and CNN. for LSTM, i have used 1 layer encoder and 1 layer decoder LSTM and 2 layer 
encoder and 2 layer decoder LSTM.
For CNN, i have used convolutional 1D layer.

After presenting the project, professor has given some update. One of them is to use EarlyStopping.

at first i have used LearningRateScheduler.

The `EarlyStopping` and `LearningRateScheduler` callbacks in Keras serve different purposes in the 
training process of a neural network, and they can affect the Root Mean Square Error (RMSE) in 
different ways.

The `EarlyStopping` callback monitors a specified metric (e.g., validation loss) during training. 
If the metric does not improve for a defined number of epochs (`patience`), training stops early. 
This helps to prevent overfitting and reduces unnecessary computation.

By stopping early, the model avoids overfitting, which often leads to better generalization on the 
validation set. This can result in a lower RMSE on unseen data compared to training for the maximum 
number of epochs, which might lead to overfitting.

The `LearningRateScheduler` adjusts the learning rate during training according to a predefined schedule 
or function. This can help the model converge more quickly and potentially reach a better minimum in the 
loss landscape.

Adjusting the learning rate can help in finding a better convergence point. If the learning rate is too high, 
the model might overshoot the minimum loss, resulting in higher RMSE. If too low, the model might converge too 
slowly or get stuck in a suboptimal minimum. A well-scheduled learning rate can lead to a better-trained model 
and a lower RMSE.

I couldn't find any publication based on this dataset. so i have followed Robust Wind Speed Forecasting: A Deep
Spatio-Temporal Approach by Mohsen Saffari, Michael Williams, Mahdi Khodayar,Miadreza Shafie-khah,João P. S. Catalão

i still couldn't finish editing the presentation and report on this project. As soon as i finish, i will upload these.

professor informed that dropping nan values is not a grood practice. in future i would like employ
to predict nan values by using machine learning technics. 
