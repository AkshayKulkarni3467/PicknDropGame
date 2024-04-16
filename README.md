![image](https://github.com/AkshayKulkarni3467/PicknDropGame/assets/129979542/97f673d5-b0e4-4728-8fef-30c4e391af2a)

Here, the q learning algorithm is implemented using a q table which holds all the states which the agent can be in.

(No of states = size*size*size*size*2 (location of carrier*location of pickup*if the carrier has picked up the client))

The algorithm picks actions using epsilon-greedy policy.
The [state,action] pair in the table is updated using the formula:

Qtable[state,action] = (1-alpha)Qtable[state,action] + alpha*(reward + gamma*next_state_reward - Qtable[state,action])
