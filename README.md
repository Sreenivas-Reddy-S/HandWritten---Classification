**📝 Handwritten Digit Classifier 🚀**

Welcome to the Handwritten Digit Classification project! 🖋️✨

This simple yet powerful neural network model is all about classifying handwritten digits. Using cool techniques and optimizations, this model achieves stellar accuracy by just looking at handwritten numbers (yep, it's like a digital handwriting reader 👀). Let's break down the magic that makes this project tick! 💥

**🔥 What’s Inside?**

Data Scaling: We scale the pixel values to a 0-1 range. Why? Because it makes the model more accurate and faster. 🚀
- X_train = X_train / 255
- X_test = X_test / 255
- Hidden Layers FTW: More layers = better performance. 💯 We added two extra hidden layers that bumped the accuracy up to 99.3% (yeah, that’s next-level).
- ReLU activation function for the first layer 🔥
- Softmax for the last layer to output probabilities like a pro 🎯
- keras.layers.Dense(100, activation = 'relu')
- keras.layers.Dense(100, activation = 'softmax')

- Optimizer Magic: We used Adam optimizer because it’s super efficient when training the model. It helps us find the best parameters and speeds up the training process. 🚀
- model.compile(optimizer = 'adam',

              loss = 'SparseCategoricalCrossentropy',

              metrics = ['accuracy'])

Visuals for the Win: To check out how well our model is doing, we use a confusion matrix and visualize it using Seaborn. This gives us a clearer view of how the model is classifying digits 🔍

- plt.figure(figsize=(10, 7))
- sn.heatmap(cm, annot=True, fmt='d')
- plt.xlabel('Predicted')
- plt.ylabel('Truth')


**🚀 Key Features:**

- Super High Accuracy: With hidden layers and some optimizations, we’re hitting up to 99.3% accuracy. 🔥
- Cool Visuals: See the model's predictions and compare them with the actual results using Seaborn heatmaps. 🔥
- Simple & Effective: This is a beginner-friendly project, but the results are solid enough to impress even the pros. 🤓

**🔧 Requirements:**

To run this project smoothly, you'll need:

- Python 3.x
- TensorFlow (for the neural network magic 🔮)
- Keras (for building the deep learning model)
- NumPy (for numerical operations 🔢)
- Matplotlib & Seaborn (for visualizations 📊)

**🚀 How to Run:**

- Clone this repo to your local machine.
- Install dependencies via pip:
- pip install tensorflow numpy matplotlib seaborn
- Run the digit_classifier.py file to see your model in action!

**✨ Final Thoughts:**

This project is perfect for anyone who wants to get their hands dirty with deep learning and neural networks. Whether you're a beginner looking to explore or someone trying to fine-tune a project to perfection, this is the one. 📈

✨ Thanks for checking this out! ✨

Stay awesome and keep building! 
