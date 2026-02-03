# Neural Network from Scratch – MNIST

This project represents **my first hands-on experience with neural networks**.  
The main goal was **not to achieve state-of-the-art accuracy**, but to **deeply understand how a neural network works internally** by implementing one **entirely from scratch** using matrix operations.

## Project Goal

The purpose of this notebook was to:
- understand how a **feedforward neural network** works
- manually implement **forward propagation**
- derive and code **backpropagation** using the **chain rule**
- work directly with **vectors and matrices**, without relying on high-level deep learning frameworks

For this reason, **no libraries such as TensorFlow, PyTorch, or Keras were used**.  
Only basic tools like NumPy and Pandas were employed.

## Dataset

The model is trained on the **MNIST (Digit Recognizer)** dataset, which consists of handwritten digit images (0–9), each represented as a vector of 784 pixel values.

The dataset comes from the *Digit Recognizer* competition on Kaggle.

## Network Architecture

The implemented neural network has the following structure:

- **Input layer**: 784 neurons (image pixels)
- **Hidden layer**: 10 neurons with ReLU activation
- **Output layer**: 10 neurons (digit classification)

Training is performed using **gradient descent**, with manual computation of:
- weight gradients
- bias gradients
- parameter updates at each iteration

## Why “from scratch”

This project is intentionally:
- **simple**
- **educational**
- **not optimized**

Some design choices (architecture size, activation functions, loss handling) were made **for learning purposes**, in order to clearly follow:
- data flow through the network
- gradient propagation
- the role of the chain rule in computing derivatives

## What I Learned

Through this project, I gained:
- a concrete understanding of **backpropagation**
- stronger intuition for **matrix-based computations**
- awareness of what deep learning libraries actually do “under the hood”

This notebook therefore represents **a starting point**, not a final or production-ready solution.

## Possible Future Improvements

- use of Softmax + Cross-Entropy loss
- mini-batch gradient descent
- data normalization
- comparison with standard deep learning frameworks

---

**Note**: this project should be viewed as a learning exercise and experimentation, not as an optimized or production-level implementation.
