# ML HACKATHON - Hangman AI Project

## Overview
This project contains an implementation of a **Smart Hangman Agent** that uses machine learning and probabilistic models to guess words efficiently. It employs Reinforcement Learning (Q-learning) and Hidden Markov Models (HMM) for prediction and decision-making.

## Key Components
- Word loading and preprocessing
- Model building: frequency models, transition probabilities
- Candidate filtering
- Guessing strategy based on frequency, HMM, and Q-values
- Reinforcement learning updates
- Caching of patterns for faster future predictions
- Evaluation and self-play for training

## Usage
1. Load your word corpus from text files (`corpus.txt` and `test.txt`)
2. Instantiate the agent and evaluator
3. Warm up the agent with self-play games
4. Evaluate the agent on test data to measure accuracy and performance

## Main Classes and Functions
- `load_words(filename)` : Load words from a text file.
- `SmartHangmanAgentV8_4` : The main agent using probabilistic and reinforcement techniques.
- `HangmanEvaluator` : Handles training, evaluation, and self-play games.

## Parameters (Adjustable)
- `WARMUP_GAMES`: Number of self-play games for warmup
- `PRUNE_TOP_K`: Pruning threshold for candidate words
- `MAX_WRONG`: Maximum wrong guesses allowed
- `LEARNING_RATE`: Learning rate for Q-learning
- `GAMMA`: Discount factor for future rewards

## Other Notes
- The model improves with increased warmup games and optimized parameters.
- Use the provided parameters for better balance between runtime and accuracy.

## License
This project is for educational purposes. Modify and extend as needed!

