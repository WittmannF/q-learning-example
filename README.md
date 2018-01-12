# Q-Learning Example
Python implementation of the example/tutorial available in this link: http://mnemstudio.org/path-finding-q-learning-tutorial.htm

The example consists in learning the path to go outside (state = 5) given any init room (from 0 to 4):
![modeling_environment_clip_image002a.gif](http://mnemstudio.org/ai/path/images/modeling_environment_clip_image002a.gif)

The states and actions can be converted to a graph where a reward is assigned if the agent reaches the target state:
![map2a.gif](http://mnemstudio.org/ai/path/images/map2a.gif)

This graph can also be converted to a Reward matrix:
![r_matrix1.gif](http://mnemstudio.org/ai/path/images/r_matrix1.gif)

The ultimate goal of Q-Learning is to learn through iteration the optimal policy to reach the way out given any start state:
![q_matrix5.gif](http://mnemstudio.org/ai/path/images/q_matrix5.gif)

Given any state, the algorithm will choose as action (next state) always the state with the highest Q-value. For example, if the initial state is 0, the next state is going to be 4 since the Q value is 80, then the next state from 4 is going to be 5 since the Q value is 100.  
