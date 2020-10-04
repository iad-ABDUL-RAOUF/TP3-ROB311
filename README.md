# TP3-ROB311
TP3 solved by madeleine BECKER and iad ABDUL RAOUF.

The code is to be found on the master branch. We successfully coded the QLearnningAgent and ApproxiamteQAgent. It runs without errors and learns correctly on the small grid. 

For the QLearningAgent, we added a setQValue(self, state, action, value) to access the Q values more easily. The state-action tuple is made of the pacman and first ghost positions and action name. For sake of simplicity, the agent only knows the position of one ghost and it doesn't know the position of food, and therefore will not perform good at all on more complexe grid with a lot of food and multiple ghosts. For instance it has worse results on the medium classic grid with two ghosts. We understand that it is not intrinsic to the Q-learning method. We made this choice in order to move on to the approximate agent quickly. Further improvement could be made.

For the ApproximateQAgent, we used the SimpleExtractor to determine the features used, therefore it adapts itself to different sizes of grid and different numbers of ghosts. 

**Results :**
* After 2000 trainings, the QlearningAgent (PacmanQAgent) wins all 10 games on the small grid (501,2 points on average). As expected, it lost all 10 games on the medium classic grid (-163.3 points on average).
* After 2000 trainings, the ApproximateQAgent wins 9 games out of 10 on the small grid (402.3 points on average) and on the medium classic grid (1182 points on average).
