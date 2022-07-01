# HandWritten---Classification

Using a simple neutral network classifying handwritten digits

Scaling is technique that improves the accuracy of the model, we scaled the values to '0-1'.

   X_train = X_train/255
   X_test = X_test/255

Adding hidden layers improves the performance of the model, Here using sigmoid activation will improve the performance to 99.2% where as using softmax improves to 99.3%
we have added 2 extra layers, which in return gives the highest accuracy.

   keras.layers.Dense(100, activation = 'relu')
   keras.layers.Dense(100, activation = 'softmax')
   
Optimizer allows us to train efficiently, when the backward propagation and the training is going on.
It will allow us to reach to global optima in efficient way.

model.compile(optimizer = 'adam',
              loss = 'SparseCategoricalCrossentropy',
              metrics = ['accuracy'])

In Numpy-> we have argmax to find the maximum element and returns the index of it.

Used Seaborn visualization to get a clear view of the output.

plt.figure(figsize = (10,7))
sn.heatmap(cm, annot = True, fmt = 'd')
plt.xlabel('Predicted')
plt.ylabel('Truth')

