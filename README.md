# Tic Tac Toe with Graph Neural Network (GNN)

This project is an implementation of the classic Tic Tac Toe game, enhanced with AI capabilities powered by a Graph Neural Network (GNN). The AI plays as 'O' and attempts to make optimal moves based on the game state.

## Features

- **Interactive UI:** Play Tic Tac Toe against the AI through an intuitive, grid-based interface.
- **AI with GNN:** The AI player uses a trained GNN model to predict the best moves.
- **Real-time Updates:** The game UI updates in real-time with each move.
- **Winner Detection:** The game automatically detects when a player wins or when the game ends in a draw.

## Installation

To run this project, you will need to have the following dependencies installed:

- Python 3.x
- Jupyter Notebook or Google Colab
- PyTorch
- PyTorch Geometric
- ipywidgets

You can install the required Python packages using the following commands:

```bash
pip install torch
pip install torch-geometric
pip install ipywidgets
```

## How to Run

1. **Clone or Download the Repository:**

   ```bash
   git clone https://github.com/TriparnaR/Tic-Tac-Toe-GNN.git
   cd Tic-Tac-Toe-GNN
   ```

2. **Open the Jupyter Notebook:**

   You can open the Jupyter Notebook or Google Colab file where the code is located.

3. **Load the Model:**

   Ensure that the pre-trained GNN model (`GNN.ipynb`) is available in the same directory. If the model file is missing, the game will not load correctly.

4. **Run the Cells:**

   Execute all the cells in the notebook to start the game.

5. **Play the Game:**

   - The game UI will be displayed, and you can start playing by clicking on the grid.
   - The AI will automatically make moves after you.

## How the GNN Works

The GNN model is trained to evaluate the Tic Tac Toe board as a graph, where each cell is represented as a node. The model predicts the best possible move for the AI based on the current game state. It uses two layers of Graph Convolutional Networks (GCNs) followed by fully connected layers to output the optimal move.

### Model Architecture:

- **Input:** 9 nodes (representing the 3x3 grid)
- **Graph Convolutional Layers:** 2 layers with ReLU activation
- **Fully Connected Layers:** 2 layers with output for 9 possible moves

## Project Structure

```plaintext
Tic-Tac-Toe-GNN/
│
├── GNN.ipynb                     # Pre-trained GNN model file
├── TIC TAC TOE (UI Design).png   # UI Design of the game
├── Tic tac initial result.csv    # Containing Data set
├──tic_tac_toe.py                 # Google Colab containing the game and model code
└── README.md                     # Project documentation

```

## Customization

- **UI Design:** You can modify the UI elements (e.g., button styles, colors) by adjusting the HTML/CSS within the `create_ui()` function.
- **Model:** If you want to improve the AI's performance, you can retrain the GNN model with additional data or tweak the architecture.

## Future Improvements

- **Advanced AI:** Experiment with more advanced GNN architectures or training techniques to improve the AI's decision-making.
- **Multiplayer Mode:** Add support for playing against another human player.
- **Mobile-Friendly UI:** Make the game interface responsive for better usability on mobile devices.

## Credits

- **PyTorch** and **PyTorch Geometric** for providing the tools to implement the GNN model.
- **ipywidgets** for enabling the interactive UI within Jupyter Notebooks.

