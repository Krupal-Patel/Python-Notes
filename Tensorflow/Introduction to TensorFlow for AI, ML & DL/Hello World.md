# Simple TensorFlow Model: Learning y = 2x - 1

This guide walks through a basic TensorFlow script that trains a model to learn a straight-line relationship (y = 2x - 1) from data. We’ll explain the code line-by-line to show how it works.

## The Code

Here’s the full script we’ll break down:

```python
import tensorflow as tf
import numpy as np

# Declare model inputs and outputs for training
xs = np.array([-1.0,  0.0, 1.0, 2.0, 3.0, 4.0], dtype=float)
ys = np.array([-3.0, -1.0, 1.0, 3.0, 5.0, 7.0], dtype=float)

# Build a simple Sequential model
model = tf.keras.Sequential([
    # Define the input shape
    tf.keras.Input(shape=(1,)),
    # Add a Dense layer
    tf.keras.layers.Dense(units=1)
    ])

# Compile the model
model.compile(optimizer='sgd', loss='mean_squared_error')

# Train the model
model.fit(xs, ys, epochs=500)

# Make a prediction
print(f"model predicted: {model.predict(np.array([10.0]), verbose=0).item():.5f}")

# Simple TensorFlow Model: Explanation

This guide explains a basic TensorFlow script that trains a model to learn the straight-line relationship `y = 2x - 1`. Each step is described below with a focus on what it does and why it matters.

```Python
import tensorflow as tf
import numpy as np
```

## **Import TensorFlow**

- **What it does**: Imports the TensorFlow library, our toolbox for building and training machine learning models.
- **Simple terms**: Like opening your kitchen cabinet to get all your cooking tools.

## **Import NumPy**

- **What it does**: Imports NumPy, a library for handling numbers and arrays efficiently—TensorFlow works well with it.
- **Simple terms**: Like grabbing a calculator to help with math while cooking.

```Python
# Declare model inputs and outputs for training
xs = np.array([-1.0,  0.0, 1.0, 2.0, 3.0, 4.0], dtype=float)
ys = np.array([-3.0, -1.0, 1.0, 3.0, 5.0, 7.0], dtype=float)
```

## **Define Input Data (xs)**

- **What it does**: Creates an array of input data (x-values): -1, 0, 1, 2, 3, 4. Ensures they’re decimals with a specific data type.
- **Simple terms**: Lists the ingredients—your “x” numbers the model will learn from.

## **Define Output Data (ys)**

- **What it does**: Creates an array of output data (y-values): -3, -1, 1, 3, 5, 7. These are the “correct answers.”
- **Simple terms**: The results you want—like “when x is 2, y should be 3.”

```Python
# Build a simple Sequential model
model = tf.keras.Sequential([
```

## **Start Sequential Model**

- **What it does**: Starts a simple model using Keras (part of TensorFlow). “Sequential” means layers stack one-by-one.
- **Simple terms**: Like starting a recipe—step 1, step 2, etc.

```Python
    # Define the input shape
    tf.keras.Input(shape=(1,)),
```

## **Define Input Layer**

- **What it does**: Defines the input layer, saying each data point is one number.
- **Simple terms**: Tells the model, “expect one ingredient at a time” (e.g., just x).

```Python
    # Add a Dense layer
    tf.keras.layers.Dense(units=1)])
```

## **Add Dense Layer**

- **What it does**: Adds a “Dense” layer with 1 neuron. This learns a straight-line equation (y = mx + b).
- **Simple terms**: The chef who mixes one input (x) to guess one output (y).

## **Close Model Definition**

- **What it does**: Closes the model definition—everything inside is set.
- **Simple terms**: Says, “recipe done, ready to cook!”

```Python
# Compile the model
model.compile(optimizer='sgd', loss='mean_squared_error')
```

## **Compile the Model**

- **What it does**: Sets up the model with:
  - A slow weight-tweaking method called Stochastic Gradient Descent.
  - A loss measurement that averages squared differences (Mean Squared Error).
- **Simple terms**: Picks a coach to fix mistakes and a scorecard to track errors.

```Python
# Train the model
model.fit(xs, ys, epochs=500)
```

## **Train the Model**

- **What it does**: Trains the model with the input and output data for 500 rounds (epochs), adjusting weights to lower loss.
- **Simple terms**: Practices the recipe 500 times—each time, the chef gets better.

```Python
# Make a prediction
print(f"model predicted: {model.predict(np.array([10.0]), verbose=0).item():.5f}")
```

## **Make a Prediction**

- **What it does**: 
  - Guesses the output for an input of 10.
  - Keeps the process quiet (no extra output).
  - Extracts the single number result.
  - Formats it to 5 decimal places.
- **Simple terms**: Tests the chef with a new input (10) and prints the guess (should be ~21).

## What’s Happening?

- **The Pattern**: The data follows y = 2x - 1 (e.g., 2*2 - 1 = 3).
- **Training**: The model learns this line over 500 rounds.
- **Prediction**: For an input of 10, it predicts ~21 (2*10 - 1 = 21), showing it worked!

This explanation outlines a great intro to TensorFlow—training a tiny model to learn a straight line from data.
