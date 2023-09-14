# flappy-bird_Reinforcement_Learning
This code demonstrates the training of an AI agent to play the popular game "Flappy Bird" using a technique called Reinforcement Learning (RL). The objective is to teach the agent to control a bird to navigate through a series of pipes, maximizing its score by avoiding collisions.
# Flappy Bird Reinforcement Learning - Technical Report
##Introduction
This technical report provides an in-depth understanding of the Flappy Bird Reinforcement Learning code. It describes the code's structure, key components, and how it uses NEAT to train AI agents to play the game.

## Code Structure
The code consists of several key components:

Bird Class: Represents the bird character, handling its movement, animation, and collision detection.
Pipe Class: Represents the pipes the bird must navigate through, managing their movement and collision detection.
Base Class: Represents the moving floor in the game, creating the illusion of scrolling.
NEAT: The neuroevolution framework used for evolving neural networks.
Main Game Loop: Orchestrates the game and AI training process.
Bird Class
Bird represents the flappy bird character.
jump() method makes the bird jump.
move() method simulates bird movement under gravity.
draw() method handles bird animation and drawing.
get_mask() method returns the mask for collision detection.
Pipe Class
Pipe represents the pipes the bird must navigate.
set_height() sets the height and positions of the pipes.
move() method moves the pipes from right to left.
draw() method handles the drawing of top and bottom pipes.
collide() method checks for collisions between bird and pipes.
Base Class
Base represents the moving floor in the game.
move() method simulates floor scrolling.
draw() method handles drawing the floor.
NEAT (NeuroEvolution of Augmenting Topologies)
NEAT is used to evolve neural networks controlling the bird.
Genetic algorithm is applied to select the best-performing networks.
Fitness is assigned based on the bird's performance.
Main Game Loop
Orchestrates the game and AI training.
Manages display, game mechanics, and fitness evaluation.
Utilizes NEAT to evolve bird AI agents.
How It Works
AI agents control birds with random neural networks.
Fitness is determined by bird performance.
Higher fitness agents have better chances of passing networks to the next generation.
Multiple generations improve AI over time.
Training Parameters
Population Size: Number of AI agents per generation.
Fitness Function: Evaluation of agent performance.
Generations: Number of training iterations.
Execution
Run the main script to start training AI agents.
Ensure required libraries and image resources are available.
Dependencies
Python
Pygame (for graphics)
NEAT-Python (for NEAT implementation)

# Conclusion
The Flappy Bird Reinforcement Learning code demonstrates the use of NEAT to train AI agents to play a game. This report provides insights into its structure and functionality, aiding developers in understanding and extending the code.

# Flappy Bird Reinforcement Learning: Training an AI Bird
## Introduction
This code demonstrates the training of an AI agent to play the popular game "Flappy Bird" using a technique called Reinforcement Learning (RL). The objective is to teach the agent to control a bird to navigate through a series of pipes, maximizing its score by avoiding collisions.

## Key Components
Bird Class
Represents the flappy bird character.
Handles bird movement, jumping, animation, and collision detection.
Uses image sprites for bird animation.

## Pipe Class
Represents the pipes that the bird must navigate through.
Manages pipe movement, drawing, and collision detection.
Includes top and bottom pipes with a gap in between.

## Base Class
Represents the moving floor in the game.
Simulates scrolling to give the illusion of movement.
Utilizes image sprites for the floor.
NEAT (NeuroEvolution of Augmenting Topologies)
Genetic algorithm framework for evolving neural networks.
Manages the evolution of neural networks controlling the bird.
Assigns fitness scores to genomes based on their performance.

## Main Game Loop
Orchestrates the game and AI training process.
Controls the display, game mechanics, and fitness evaluation.
Utilizes NEAT to evolve bird AI agents.

## How It Works
Bird AI agents are initialized with random neural networks.
In each generation, AI agents control birds to play the game.
The fitness of each agent is determined by its performance in the game.
Agents with higher fitness scores have a higher chance of passing their neural network weights to the next generation.
The process continues for multiple generations, allowing the AI to improve over time.

## Training Parameters

Population size: The number of AI agents in each generation.
Fitness function: How well an agent performs in the game.
Generations: The number of generations the AI will train for.

## Execution
To run the code, execute the main script. Ensure that the required libraries and resources (images) are available.

## Dependencies
Python
Pygame (for game graphics)
NEAT-Python (for NEAT implementation)
