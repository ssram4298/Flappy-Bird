
# Flappy Bird AI

This project is an implementation of the Flappy Bird game using Pygame and NEAT (NeuroEvolution of Augmenting Topologies) to train a neural network to play the game.

## Features

- **Flappy Bird Gameplay:** Classic Flappy Bird game recreated using Pygame.
- **Neuroevolution:** Uses the NEAT algorithm to evolve neural networks that learn to play the game.
- **Visualization:** Real-time display of the game with the AI birds learning and improving over generations.

## Requirements

- Python 3.6+
- Pygame
- NEAT-Python

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/flappy-bird-ai.git
   cd flappy-bird-ai
   ```

2. Install the required packages:
   ```sh
   pip install pygame neat-python
   ```

## Usage

1. Ensure the images for the bird, pipes, base, and background are located in an `imgs` folder in the same directory as the script.
2. Run the script:
   ```sh
   python flappy-bird.py
   ```

The AI will start learning to play the game. You can observe the progress in real-time.

## Configuration

The NEAT configuration file `config-feedforward.txt` contains various parameters for the NEAT algorithm. Here are some key parameters:

- **fitness_criterion:** Criterion for selecting the fittest genomes.
- **pop_size:** Population size for each generation.
- **num_inputs:** Number of inputs to the neural network.
- **num_outputs:** Number of outputs from the neural network.

For more details, refer to the NEAT documentation.

## Code Overview

- `flappy-bird.py`: Main script containing the game and NEAT implementation.
- `config-feedforward.txt`: Configuration file for NEAT.

### Main Classes and Functions

- **Bird**: Class representing the bird in the game.
- **Pipe**: Class representing the pipes in the game.
- **Base**: Class representing the base of the game.
- **draw_window**: Function to draw the game window.
- **eval_genomes**: Function to evaluate the genomes in each generation.
- **run**: Main function to run the NEAT algorithm.

## License

This project is licensed under the MIT License.
