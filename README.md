# RNN From Scratch - Word Prediction

This project implements a simple Recurrent Neural Network (RNN) from scratch using only NumPy. The model is trained to predict the fourth word in a sentence of four words (e.g., "I love deep learning").

## 🔧 Model Overview
- **Input**: A sequence of 3 words (converted to one-hot vectors).
- **Architecture**:
  - One hidden layer with `tanh` activation
  - Manual forward and backward pass
  - Softmax for output prediction
- **Parameters**:
  - `W1`: Input to hidden weights
  - `W2`: Hidden to hidden weights
  - `W3`: Hidden to output weights
  - `b1`, `b2`: Bias terms
  - ![image](https://github.com/user-attachments/assets/d3aff5db-7064-46ad-aaed-55af49194f2b)


## 🔁 Training
- The model uses manual backpropagation through time (BPTT).
- Loss is not explicitly calculated but gradients are computed from the difference between predicted and target one-hot vectors.
- Parameters are updated using simple gradient descent.
- You can train for multiple epochs to observe learning behavior.

## 📄 Files
- `rnn_train.py`: Python file containing full training loop.
- You can run it directly with Python 3: `python rnn_train.py`

## 📝 Example Output
During training, you will see:
- Hidden state at each time step
- Softmax probabilities
- Predicted word
- Gradients and updated weights

## 🚀 Future Improvements
- Add support for more training data
- Use loss tracking and graphing
- Extend to larger vocabulary or more complex sequences

