# Rock-Paper-Scissors with RNN Prediction

This project uses a Recurrent Neural Network (RNN) to predict the player's next move in the classic game of Rock-Paper-Scissors. By analyzing the sequence of previous moves, the model attempts to learn patterns and improve its predictions, making the game more challenging for the user.

## Overview

The Recurrent Neural Network in this project is trained to predict the next move (rock, paper, or scissors) based on the player's move history. The model processes sequential data, capturing dependencies between the previous moves and predicting the next one. This makes the gameplay dynamic, as the AI learns from the player's strategies over time.

### Key Features
- **PyTorch-based RNN Model:** The RNN model is built using PyTorch and processes sequences of player moves to predict the next move.
- **Real-time AI Learning:** The AI tracks the player's moves, updates its internal memory (hidden state), and adjusts predictions based on learned patterns.

## Model Details

- **Input Size:** 3 (representing `rock`, `paper`, and `scissors`)
- **Hidden Layers:** 2 layers for improved learning
- **Dropout:** 0% (no dropout)
- **Learning Rate:** 0.5 (adjustable)
- **Weight Decay:** 1e-5 to prevent overfitting

The RNN processes the sequence of moves and outputs a probability distribution over the possible next moves. The AI then selects its next move based on these probabilities.

## Setup Instructions

To run this project locally, follow the steps below:

### 1. Clone the Repository
```
git clone https://github.com/your-username/rps-rnn.git
cd rps-rnn
```

### 2. Install Dependencies
Ensure that you have Python 3.7+ installed. Install the required Python packages:
```
pip install torch ipywidgets
```

### 3. Run the Notebook
The interactive game is implemented in a Jupyter Notebook. Start the Jupyter Notebook server by running:
```
jupyter notebook
```
Open the `rock_paper_scissors_RNN.ipynb` notebook to start the game.

Or open it with VSCode.

## How It Works

1. The player selects either `Rock`, `Paper`, or `Scissors` through the UI.
2. The RNN model predicts the player's next move based on the sequence of previous moves.
3. The AI selects its move, and the game determines the outcome (win, lose, or tie).
4. The player's past moves are stored, and the AI continually learns patterns to improve its predictions.

## Future Improvements

- **Model Training:** Improve the AI's prediction accuracy by fine-tuning the hyperparameters and exploring more sophisticated RNN variants such as LSTM or GRU.
- **Enhanced Game Strategy:** Incorporate reinforcement learning to enable the AI to learn more complex strategies.

## Contributions

Feel free to contribute to this project! Whether it's improving the model, adding new features, or fixing bugs, all contributions are welcome. Please open a pull request or create an issue for any suggestions or bugs.
