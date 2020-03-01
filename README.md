README
------------------------------------------------------------------------
Run the whole notebook to get the answers with videos.
All videos are saved in the videos directory.
------------------------------------------------------------------------
In this notebook we train a rat to eat a maximum amount of cheese in a grid, with also the presence of poisonous cells.
We use the DQN algorithm.
------------------------------------------------------------------------
Hints on the code:
In question 6, we define a memory to store transitions and use them in the updates. The memory with a maximum size and a FIFO design.
------------------------------------------------------------------------
In question 7, we implement the DQN update rules and the state-action value function is designed with a neural net with one hidden layer fully connected. It takes as input the state and returns the value function for all possible actions.
In question 8, we use a CNN to model the state-action value function.
------------------------------------------------------------------------
The approach above is poor because the rat gets stuck when there is no nearby positive reward. We encourage more exploration in what follows by adding a negative reward to previously visited cells and by using a decaying epsilon factor.