# TP3-ROB311
TP3 solved by madeleine BECKER and iad ABDUL RAOUF.

The code is to be found on the master branch. We successfully coded the QLearnningAgent and ApproxiamteQLearningAgent. It runs without errors and learns correctly on the small grid. 
For the QLearningAgent, we added a setQValue(self, state, action, value) to access the Q values more easily. But in this version, the agent only knows the position of one ghost. 
For the ApproximateQAgent, we used the SimpleExtractor to determine the features used, therefore it adapts itself to different sizes of grid and different numbers of ghosts. 
